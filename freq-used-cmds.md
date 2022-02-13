### Dev Resources
[Jenkins - Azure](http://ops-server.westus2.cloudapp.azure.com:8080/login?from=%2F)<br>
[Jenkins - AWS](https://build.rythm.cc/login?from=%2F)<br>
[Kafka](https://login.confluent.io/login?state=g6Fo2SBlSTBhaTlTRlNvUUViQmVsV0pjXzhrZk5ZTE9VUHBrcaN0aWTZIHJFQUtobVlEaUlQTjUxYjFlalNJWmtWWktNN3htdGYzo2NpZNkgbDJoT3AwUzB0a1NCMFRGdHZJWWZaWjlFYUtGdnJTYzY&client=l2hOp0S0tkSB0TFtvIYfZZ9EaKFvrSc6&protocol=oauth2&response_type=id_token&redirect_uri=https%3A%2F%2Fconfluent.cloud%2Fauth_callback&nonce=Ik.mzhx2hxlwDSKCz7Kjmus5hDKAjscG&scope=openid%20profile%20email&auth0Client=eyJuYW1lIjoiYXV0aDAuanMiLCJ2ZXJzaW9uIjoiOS4xNC4wIn0%3D)<br>
[Diagrams](https://lucid.app/documents#/dashboard)

### shell
echo -n "username:123123adsfasdf123123" | base64  


### Python
#### Jupyter
Start jupyter on server - headless  
nohup jupyter notebook --no-browser --port=8888 &  

Port forward from workstation  
ssh -L 8888:localhost:8888 brandon@20.69.90.222  
[running notebook on server](https://towardsdatascience.com/running-jupyter-notebooks-on-remote-servers-603fbcc256b3)  


### Java
**Java Home**<br>
/Library/Java/JavaVirtualMachines/jdk-15.0.1.jdk/Contents/Home<br>
brew install maven<br>
brew install gradle<br>

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

