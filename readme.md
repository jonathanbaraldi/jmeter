jmeter


https://sqa.stackexchange.com/questions/20831/how-to-load-100-urls-as-http-request-in-jmeter



https://github.com/iorga-group/jmeter-docker/blob/master/README.md

ssh -i rancher2.pem linux@186.200.35.25


## >>>>>>> CLUSTER KUBERNETES

rancher server = 186.200.35.174

ssh -i rancher2.pem linux@186.200.35.173
ssh -i rancher2.pem linux@186.200.35.87
ssh -i rancher2.pem linux@186.200.35.150



$ docker rm -f $(docker ps -qa)
$ docker rmi -f $(docker images -q)
$ docker volume rm $(docker volume ls)
$ systemctl stop docker
$ for mount in $(mount | grep tmpfs | grep '/var/lib/kubelet' | awk '{ print $3 }') /var/lib/kubelet /var/lib/rancher; do umount $mount; done
$ rm -rf /etc/ceph /etc/cni /etc/kubernetes /opt/cni /opt/rke /run/secrets/kubernetes.io /run/calico /run/flannel /var/lib/calico /var/lib/etcd /var/lib/cni /var/lib/kubelet /var/lib/rancher/rke/log /var/log/containers /var/log/pods /var/run/calico
$ systemctl start docker



Subscription ID* 
Client ID* 
Client Secret*



### >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

$ kubectl apply -f app.yml




./build-and-run.sh /workdir/teste2.jmx 01

# AWS



ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@54.233.234.248
ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@18.231.114.143
ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@18.228.153.225
ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@52.67.86.238

ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@18.228.152.121
ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@54.207.95.146
ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@52.67.77.218
ssh -i /Users/jonathanbaraldi/Dropbox/Jonathan2018/TSE/jmeter-aws.pem ec2-user@18.231.104.135





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

















