备份系统已安装软件的清单，采用如下命令 （dpkg命令后的参数前是两个减号“-”）：
sudo dpkg --get-selections > ~/Documents/App_Addon_List/Ubuntu-app-backup-list.txt

恢复安装软件，采用如下命令：
sudo dpkg --set-selections < ~/Documents/App_Addon_List/Ubuntu-app-backup-list.txt && sudo apt-get dselect-upgrade