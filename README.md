#### mac 指令集

+	mac设置终端（terminal）tab键忽略大小写
>	echo 'set completion-ignore-case on' >> ~/.inputrc 

    没有.inpoutrc文件系统会自动创建（linux下一样）

+	创建软连接（sublime）
>	sudo ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl

+	安装 Homebrew
>	/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

+	mac管理员被搞成普通用户了。没有权限
	
	管理重启  按着`command + s` 等待出现命令行 root#  接着输入
	>	/sbin/mount -uaw

	>	rm var/db/.AppleSetupdone

	>	reboot

	重启系统 在重新创建一个管理员用户，创建号后，把原来的账号设置为管理员，退出登录，登录的帐号

+	mac 链接连接远程服务器
>	sudo -i
>	ssh xxx@127.0.0.1
