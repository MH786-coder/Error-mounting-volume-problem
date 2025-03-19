# Error-mounting-volume-problem

## We should install the requirements
```
sudo apt-get install nfs-common
sudo apt-get install cifs-utils
```
NOTE : Don't miss the any requirements, because it may not works properly 

____

# Let's start to fix it

After install the requirements,we should find your disk name by,
```
sudo fdisk -l
```
Find your disk, which has the error to mounting
we'll find like this,
```
Disk /dev/[your_disk_name]
```

Finally,run
```
sudo ntfsfix -d /dev/[your_disk_name]
```
Let's try to open your disk,may you have a good result
