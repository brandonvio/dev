### Powershell Commands
**Remove folder and all files recursively**<br>
Remove-Item -Recurse -Force {folder-name}<br>

###  CDK Commands
**Install the AWS CDK**<br>
npm install -g aws-cdk

**Initialize CDK project**<br>
cdk init --language typescript<br>

**Most common used CDK modules**<br>
npm install @aws-cdk/aws-s3, @aws-cdk/aws-dynamodb, @aws-cdk/aws-cloudfront, @aws-cdk/aws-route53, @aws-cdk/aws-cognito, @aws-cdk/aws-ec2, @aws-cdk/aws-cloudfront-origins<br>

###  AWS
#### AWS CLI commands
**sync contents of folder to S3**<br>
aws s3 sync build/ s3://{bucket-name} --acl public-read<br>
aws s3 sync static/ s3://{bucket-name} --acl public-read<br>

**list content of bucket**<br>
aws s3 ls s3://{bucket-name}<br>

#### AWS [OrganizationAccountAccessRole]

###  git
#### github hub
**created private repository**<br>
hub create -p<br>

**push branch to newly created repository**<br>
git push --set-upstream origin master<br>

###  SSH
**Create an SSH key**<br>
ssh-keygen -t rsa -b 4096 -C "{email}"<br>

**Add key**<br>
ssh-add id_rsa
