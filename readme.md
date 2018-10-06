jmeter


https://sqa.stackexchange.com/questions/20831/how-to-load-100-urls-as-http-request-in-jmeter



https://github.com/iorga-group/jmeter-docker/blob/master/README.md

ssh -i rancher2.pem linux@186.200.35.25

./build-and-run.sh /workdir/teste2.jmx 01

# AWS


ssh -i jmeter-aws.pem ec2-user@18.231.190.163
ssh -i jmeter-aws.pem ec2-user@18.228.137.110
ssh -i jmeter-aws.pem ec2-user@18.228.6.155 


ssh -i jmeter-aws.pem ec2-user@18.228.136.55
ssh -i jmeter-aws.pem ec2-user@18.228.156.16


## >>>>>>
#!/bin/bash
yum install docker -y
yum install git -y
git clone https://github.com/jonathanbaraldi/jmeter
yum install epel-release -y
yum install -y python-pip
pip install docker-compose -y
yum upgrade python* -y
pip uninstall docker-compose
pip install docker-compose==1.9.0
cd jmeter/docker-compose
systemctl start docker 
docker-compose build
./build-and-run.sh /workdir/teste2.jmx 01