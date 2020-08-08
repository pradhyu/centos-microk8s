https://snapcraft.io/install/microk8s/centos

reboot to make snapd commands work 


microk8s start 



[centos@centos8 ~]$ microk8s status
Insufficient permissions to access MicroK8s.
You can either try again with sudo or add the user centos to the 'microk8s' group:

    sudo usermod -a -G microk8s centos
    sudo chown -f -R centos ~/.kube

# debugging the tcp packates with tcpdump 
sudo tcpdump -n -tttt -i enp0s3  icmp