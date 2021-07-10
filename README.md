# P4-test

Follow this tutorial to start with P4 - https://opennetworking.org/news-and-events/blog/getting-started-with-p4/

# for creating VM using virt-install in server - https://www.server-world.info/en/note?os=Ubuntu_20.04&p=kvm&f=2

$ virt-install \
--name ubuntu2004 \
--ram 4096 \
--disk path=/var/kvm/images/ubuntu2004.img,size=20 \
--vcpus 2 \
--os-variant ubuntu20.04 \
--network bridge=br0 \
--graphics none \
--console pty,target_type=serial \
--location /home/ubuntu-20.04-live-server-amd64.iso,kernel=casper/vmlinuz,initrd=casper/initrd \
--extra-args 'console=ttyS0,115200n8 serial' 


