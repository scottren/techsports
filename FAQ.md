# Docker

* Docker 启动失败

关键错误信息：

registry.sefon.com dockerd-current[6374]: Error starting daemon: SELinux is not supported with the overlay2 graph driver on this kernel. Either boot into a newer kernel or disabl...nabled=false)

解决方法：

编辑 Docker 配置文件： /etc/sysconfig/docker，修改 --selinux-enabled=false

OPTIONS='--selinux-enabled=false --log-driver=journald --signature-verification=false --registry-mirror=https://fzhifedh.mirror.aliyuncs.com --insecure-registry=registry.sese.com' 



