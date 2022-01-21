# bash_notes
<p align="center">My frequently used bash commands</p>
```
sudo sync && sudo sysctl -w vm.drop_caches=3
#Clear OS cache
ls | xargs du -hs
#List folders with its disk size
sudo ntpdate -b 2.amazon.pool.ntp.org 
#sync an EC2 instance time
find /home/ubuntu/MyFolder/files/* -mmin +400 -type f -delete #locate and delete files older than 400 minutes
dd if=/dev/zero of=/dev/null #stress CPU
```


## Increase disk size without reboot (after EC2, Google VM or VMware storage expansion)
> sudo file -s /dev/xvd*
> df -H
> lsblk
> sudo growpart /dev/xvda1
> sudo resize2fs /dev/xvda1

https://img.shields.io/twitter/follow/demuxer?style=social
