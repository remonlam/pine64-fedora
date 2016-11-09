## Install Fedora trough CentOS-7

### should be run as root
nano /etc/yum.repos.d/CentOS-Base.repo

[base]
name=FedoraOS-$releasever - Base
baseurl=http://dl.fedoraproject.org/pub/fedora-secondary/releases/23/Everything/aarch64/os/
gpgcheck=0

mkdir FedoraRootFS

yum groupinstall "Minimal Install" --installroot=/home/testuser/FedoraRootFS/
