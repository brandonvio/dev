### Dev Resources
[Azure Jenkins](http://ops-server.westus2.cloudapp.azure.com:8080/login?from=%2F)<br>
[AWS Jenkins](https://build.rythm.cc/login?from=%2F)<br>

### Powershell Commands
**Remove folder and all files recursively**<br>
Remove-Item -Recurse -Force {folder-name}<br>

### Installs
**TypeScript**<br>
npm install -g typescript<br>
npm install -g aws-cdk

###  CDK Commands
**Install the AWS CDK**<br>

**Initialize CDK project**<br>
cdk init --language typescript<br>

**Most common used CDK modules**<br>
npm install @aws-cdk/aws-s3 @aws-cdk/aws-dynamodb @aws-cdk/aws-cloudfront @aws-cdk/aws-route53 @aws-cdk/aws-cognito @aws-cdk/aws-ec2 @aws-cdk/aws-cloudfront-origins @aws-cdk/aws-elasticloadbalancingv2 @aws-cdk/aws-elasticloadbalancingv2-targets @aws-cdk/aws-route53 @aws-cdk/aws-certificatemanager @aws-cdk/aws-route53-targets @aws-cdk/aws-msk @aws-cdk/aws-codepipeline @aws-cdk/aws-codepipeline-actions @aws-cdk/aws-codebuild 	@aws-cdk/aws-iam @aws-cdk/aws-ecs @aws-cdk/aws-ecs-patterns @aws-cdk/aws-ecr<br>

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

### Ports
sudo lsof -i -P -n | grep LISTEN<br>
sudo netstat -tulpn | grep LISTEN<br>
sudo lsof -i:22 ## see a specific port such as 22 ##<br>
sudo nmap -sTU -O IP-address-Here<br>


### Jenkins
**Restart Jenkins**<br>
sudo /etc/init.d/jenkins restart<br>

**Get initial password**<br>
sudo cat /var/lib/jenkins/secrets/initialAdminPassword

