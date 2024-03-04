AWS Serverless Application Model (SAM) is a framework that simplifies building and deploying serverless applications on AWS. It extends [[CloudFormation]] with a simplified syntax for defining serverless resources like Lambda functions and API Gateway APIs. SAM enables developers to define resources in a single YAML or JSON template, streamlining infrastructure management. It also provides local development tools for testing serverless applications locally before deployment, speeding up the development cycle.

Documentation: [SAM Reference](https://aws.amazon.com/serverless/sam/)
___
### Overview
#### CLI Commands

The package command is used to package a yaml template into a SAM compatible template, and uploads it to an s3 bucket.
```bash
sam package \
	--template-file <template-file> \
	--output-template-file <output-file> \
	--s3-bucket <bucket-name>
```

The deploy command takes the packaged SAM template and deploys the package to your AWS account.
```bash
sam deploy \
	--template-file <packaged-file> \
	--stack-name <stack-name> \
	--capabilities <capability-iam>
```

___
