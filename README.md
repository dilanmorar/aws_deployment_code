## How to get in machine

copy files to AWS
scp -i ~/.ssh/keyname.pem /files/you/want/copied ubuntu@ip:/where/you/want/files/in/machine

go into machine
ssh -i ~/.ssh/keyname.pem ubuntu@ip

sed -i -e 's/\r$//' jenkins.sh
cd /environment/app
./jenkins.sh


# AWS

# CI
test 10

# CD

## Getting admin password

ip:8080


type in the following code
```
cat /var/log/jenkins/jenkins.log
```
copy and paste the output into the

When in Jenkins

manage jenkins --> manage plugins
go available and search for nodejs

go back to dashboard

select new item
enter item name

choose freestyle project

General:
write a description

select github project tick box

enter the project url

Source code management:

repository url in ssh

add key
select kind ssh username with private keys
private key select enter directly
create keys
```
ssh-keygen -t rsa
```
copy and paste private keys
private key
specify branch

Build:
Execute shell
```
cd starter_code
npm install
npm run test
```
save

test 5
