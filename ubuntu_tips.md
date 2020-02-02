* Ubuntu 18.04

\# 开机启动rc.local

\# 1. 创建rc.local.service

sudo ln -s /lib/systemd/system/rc.local.service /etc/systemd/system/

\# 确保内容包含[Install]内容块

[Install]  

WantedBy=multi-user.target  

Alias=rc-local.service

\# 2. 创建/etc/rc.local文件，并添加开启启动运行命令

\# 注意：在文件头添加

\#! /bin/bash

\# 修改/etc/rc.local文件执行权限

\# 3. 开启 rc.local.service 开机启动

sudo systemctl enable rc.local.service

\# 4. 启动 rc.local.service

sudo systemctl start rc.local.service

安装指定版本

sudo apt-get install package[=10.1]
