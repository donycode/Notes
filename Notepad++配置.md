用Notepad++编译运行java的设置<br>

1.在plugin manager下下载插件NppExec<br>
2.在NppExec下的Execute下编辑保存以下命令：<br>
info cnr<br>
javac -encoding UTF8 "$(FULL_CURRENT_PATH)"  
echo  
echo ===============  编译成功后开始运行  ===============  
echo 若不使用 -cp , 则需使用 cd 切换至当前目录, 或勾选 Follow CURRENT_DIRECTORY 菜单项  
echo  
java -cp "$(CURRENT_DIRECTORY)" "$(NAME_PART)"  

complie java<br>
javac -encoding UTF8 "$(FULL_CURRENT_PATH)"  

run java<br>
java -cp "$(CURRENT_DIRECTORY)" "$(NAME_PART)" 

3.在NppExec下的Advanced Option下配置与其功能名称相对应的menu item<br>
4.在Shortcut mapper下配置其快捷键<br>

