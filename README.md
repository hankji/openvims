#openvims

一个针对 PHP / Python / C 开发人员的Vim脚本

##安装步骤

    1.    git clone https://github.com/shenyubao/openvims.git .vim
    2.    cd .vim
    3.    git submodule init
    4.    git submodule update
    5.    execute the Install.sh will override your .vimrc by openvims .vimrc

##插件管理
####新增Vim插件, 使用如下命令

    git submodule add https://github.com/scrooloose/nerdcommenter.git bundle/nerdcommenter

####删除Vim插件, 使用如下命令

    1.git rm -r --cache bundle/nerdcommenter
    2.rm -rf --cache bundle/nerdcommenter
    3.修改.gitmodules ,删除相关节点

##插件使用说明    
####默认配置

    <leader> = ,   
####Conque-Shell 

    在Vim中打开Terminal的插件
    :ConqueTerm bash 打开终端
    :ConqueTermSplit 分隔窗口方式打开终端 
    
####OmniCppComplete
    
    C/C++代码自动补全增强插件

####checksyntax_vim

    语法检查插件
    F5 启用检查(文件保存后自动检查)
    
####cscope
    
    语法标签生成,代码阅读插件
    F6 生成当前项目的语法标签(cscope -bkq)
    <C + ]> 跳转定义
    <C + t> 跳转上一步
    <C + ->g: 查找函数定义
    <C + ->d: 查找函数调用
    
####easygrep

    关键字查找插件
    <leader>vv 查找关键字
    
####file-line
####fuzzyfinder
    
    文件查找插件(支持通配符) 
    F4 开启
    
####nerdcommenter

    用来给代码添加注释
    <leader>cc 添加注释
    <leader>cu 取消注释
    <leader>c<space> 添加/取消 注释
    <leader>cm 段注释
    <leader>cs 漂亮的注释
    
####nerdtree
    
    项目目录导航
    F2 开启/关闭
    ?  打开帮助
    B  显示/关闭书签
    
####snipMate
    
    代码块生成
    for/foreach/class/func + tab 生成代码段
    语法文件: ~/.vim/snippets/*.snippets
    
####solarized
    
    默认模板自带的管理插件
####space
####supertab
    
    代码自动提醒插件
####tabular

    文本对齐插件
    :Tab /=  按等号对齐
####tagbar
    
    标签阅读插件(兼容面向对象语言)
    F3 显示/关闭
####vcscommand
    
    版本控制插件(支持Git,Svn)
    :VCSAdd 向源添加文件
    :VCSAnnotate 在每行代码前显示提交者
    :VCSCommit 提交对当前文件的更改
    :VCSDelete 在源中删除当前文件
    :VCSLog 显示文件的历史更改情况
    :VCSRevert 回滚当前文件到源中历史最新版本
    :VCSReview 查看当前文件的某个特定版本
    :VCSStatus 查看当前文件的版本信息
    :VCSUnlock 撤销对当前文件的锁定
    :VCSUpdate 更新当前文件到源中版本
    :VCSVimDiff 查看当前文件与历史版本的差别

####vim-l9
####vim-powerline
    
    状态栏增强插件
