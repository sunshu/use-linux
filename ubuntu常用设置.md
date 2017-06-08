1. sublime 和 vim 设置 Tab为4个空格

* vim 可以设置 ~/.vimrc 文件或者 /etc/vimrc

    ```  
    set ts=4  
    set expandtab  
    set autoindent
    ```
* sublime 中设置 Preferences > Setting  > Default

    ```
    "tab_size": 4,  
    "translate_tabs_to_spaces": ture,
    ```
    
2. Ubuntu无法使用sudo提权提示当前用户不在sudoers文件中
   ```
   当前用户不在sudoers用户组中
   /etc/sudoers     
   ```
   
3. Ubuntu 16.04 WPS下搜狗输入法不能输入中文
   ```
   原因：环境变量未正确设置
   解决:
        $vi /usr/bin/wps
        在第一行输入 #!/bin/bash 下添加
        export XMODIFIERS="@im=fcitx"
        export QT_IM_MODULE="fcitx"
   补充：其他应用也可以这么处理，比如sublime
   ```
   
4. 安装 gnome-tweak-tool  
    ```
    sudo apt-get install gnome-tweak-tool
    或者 gsettings set com.canonical.Unity.Launcher launcher-position Bottom
    ```