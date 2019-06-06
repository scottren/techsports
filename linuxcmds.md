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

