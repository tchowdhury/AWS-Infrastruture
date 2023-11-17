# AWS CLI Commands for CloudFormation #

## Create CodePipeline Stack(s) ##

### Git Commit ###

### S3 Artifact Bucket ###

```
aws cloudformation validate-template --template-body file://2_S3ArtifactBucket.yml 

aws cloudformation create-stack --stack-name ccDemoAppBucket --template-body file://2_S3ArtifactBucket.yml --parameters file://params/2_S3ArtifactBucket-params.json 

aws cloudformation describe-stacks --stack-name ccDemoAppBucket --query "Stacks[0].StackStatus"
```

### CodeBuild ###


### CodeDeploy ###

### CodePipeline ###

### Delete Stack ###

```
aws cloudformation delete-stack --stack-name ccDemoCodePipeline

aws cloudformation delete-stack --stack-name ccDemoCodeDeploy

aws cloudformation delete-stack --stack-name ccDemoCodeBuild

aws cloudformation delete-stack --stack-name ccDemoAppBucket

aws cloudformation delete-stack --stack-name ccDemoAppRepo
```