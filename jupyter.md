* 创建默认配置文件

jupyter notebook --generate-config

* 配置项

.jupyter/jupyter_notebook_config.py

** 允许root用户启动： c.NotebookApp.allow_root = True

** 绑定IP地址： c.NotebookApp.ip = '0.0.0.0'

** 绑定端口： c.NotebookApp.port = 8888

** 无密码认证：c.NotebookApp.token = ''

** 多行输出：.InteractiveShell.ast_node_interactivity = "all"

