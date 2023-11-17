# AWS CLI Commands for CloudFormation #

## Create CodePipeline Stack(s) ##

### Git Commit ###

### S3 Artifact Bucket ###

```
aws cloudformation validate-template --template-body file://3_CodeBuild.yml

aws cloudformation create-stack --ADD YOUR STACK NAME ccDemoCodeBuild --template-body file://3_CodeBuild.yml --parameters file://params/3_CodeBuild-params.json --capabilities CAPABILITY_IAM --capabilities CAPABILITY_NAMED_IAM

aws cloudformation describe-stacks --ADD YOUR STACK NAME ccDemoCodeBuild | grep StackStatus
```

### CodeBuild ###

### CodeDeploy ###

### CodePipeline ###

### Delete Stack ###