In Kubernetes, Persistent Volumes (PV), Persistent Volume Claims (PVC), and StorageClasses (SC) work together to provide persistent storage for containers. A StorageClass defines the type of storage (like AWS EBS or NFS) and provisioning parameters, acting as a blueprint for creating dynamic Persistent Volumes. A PVC is a user's request for storage, specifying requirements such as size and access mode. Based on the PVC, Kubernetes dynamically provisions a **PV** using the defined StorageClass, or it binds the PVC to an existing PV that meets the criteria. This architecture abstracts storage management, enabling persistent data storage across pod lifecycles.

Documentation: [Persistent Volume Reference](https://kubernetes.io/docs/concepts/storage/persistent-volumes/)
___
### Overview
#### Example Templates

Volume Mounting of a Pod: [Persistent Storage Configuration](https://kubernetes.io/docs/tasks/configure-pod-container/configure-persistent-volume-storage/)

StorageClass Template:
```yaml
apiVersion: storage.k8s.io/v1
kind: StorageClass
metadata:
  name: example-storage-class
provisioner: kubernetes.io/aws-ebs
parameters:
  type: gp2
  fsType: ext4
reclaimPolicy: Retain
allowVolumeExpansion: true
volumeBindingMode: WaitForFirstConsumer
```

PersistentVolumeClaim Template:
```yaml
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: example-pvc
spec:
  resources:
    requests:
      storage: 10Gi
  storageClassName: example-storage-class
```

PersistentVolume Template:
```yaml
apiVersion: v1
kind: PersistentVolume
metadata:
  name: example-pv
spec:
  capacity:
    storage: 10Gi
  accessModes:
    - ReadWriteOnce
  storageClassName: example-storage-class
  awsElasticBlockStore:
    volumeID: vol-0abcdef1234567890
    fsType: ext4
```

Deployment Template:
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: example-deployment
spec:
  replicas: 2
  selector:
    matchLabels:
      app: my-app
  template:
    metadata:
      labels:
        app: my-app
    spec:
      containers:
      - name: app-container
        image: nginx
        volumeMounts:
        - name: app-storage
          mountPath: /usr/share/nginx/html
      volumes:
      - name: app-storage
        persistentVolumeClaim:
          claimName: example-pvc

```

___