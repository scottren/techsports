## user operations
\# create a user with specified home directory

\# useradd $user -d $home_direcotry


\# create a user with a default home directory under /home

\# useradd -m $user

\# passwd $user

\# change $home_directory

\# usermod -md $new_home_directory $user

\# create home direcotry for a existing user

\# usermod -d $home_directory $user

\# change user id

\# usermod -u $id $user

\# change user group id

\# usermod -g $group_id $user

\# directory operation

\# change owner

\# chown \<user\>:\<group\> \<directory\>

## FS Operations
\# echo "- - -"  > /sys/class/scsi_host/host0/scan # 热添加磁盘扫描

\# pvcreate /dev/sdx

\# vgcrete nfs /dev/sdx

\# lvcreate -l 100%FREE -n apps nfs

\# vgextend nfs /dev/sdy

\# lvextend -l +100%FREE /dev/nfs/apps

\# resize2fs /dev/nfs/apps

\# xfs_growfs /dev/nfs/apps

\# 查看进程打开的文件

\# lsof /nfs
