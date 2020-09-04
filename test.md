以管理员身份运行命令提示符

执行命令 bcdedit /set hypervisorlaunchtype off

重启，运行vm即可

如果想要恢复hyper启动，bcdedit / set hypervisorlaunchtype auto


export DISPLAY=$(awk '/nameserver / {print $2; exit}' /etc/resolv.conf 2>/dev/null):0

export LIBGL_ALWAYS_INDIRECT=1
