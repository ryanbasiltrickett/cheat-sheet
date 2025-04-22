A CronJob in Kubernetes is a specialized job controller used to schedule tasks to run at specific times or intervals, similar to a Unix cron job. It creates Jobs based on a defined schedule using Cron syntax. CronJobs are ideal for periodic tasks like backups, report generation, or cleaning up logs. They ensure that the tasks are run according to the schedule, and you can control the concurrency, failure handling, and history of completed jobs. Each scheduled run of the CronJob creates a new Job that will run to completion.

Documentation: [CronJob Reference](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/)
___
### Overview
### Example Template

```yaml
apiVersion: batch/v1
kind: CronJob
metadata:
  name: hello
spec:
  schedule: "5 0 * * 2"
  startingDeadlineSeconds: 30
  concurrencyPolicy: Allow
  successfulJobsHistoryLimit: 5
  failedJobsHistoryLimit: 2
  jobTemplate:
    spec:
      template:
        spec:
          containers:
          - name: hello
            image: busybox:1.28
            imagePullPolicy: IfNotPresent
            command:
            - /bin/sh
            - -c
            - date; echo Hello from the Kubernetes cluster
          restartPolicy: OnFailure
```
### CronJob Controller
- Checks every 10 seconds for Tasks
- If >100 Tasks are missed the controller won't try anymore

___