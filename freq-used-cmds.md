# Powershell Commands
## Remove folder and all files recursively
Remove-Item -Recurse -Force {folder-name}

# CDK Commands
## Install the AWS CDK.
npm install -g aws-cdk

# Initialize CDK project.
cdk init --language typescript

# Most common used CDK modules.
npm install @aws-cdk/aws-s3, @aws-cdk/aws-dynamodb, @aws-cdk/aws-cloudfront, @aws-cdk/aws-route53, @aws-cdk/aws-cognito, @aws-cdk/aws-ec2

# AWS
## AWS CLI commands
### sync contents of folder to S3
aws s3 sync build/ s3://{bucket-name} --acl public-read
aws s3 sync static/ s3://{bucket-name} --acl public-read

### list content of bucket
aws s3 ls s3://{bucket-name}
