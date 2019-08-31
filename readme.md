##第一个git
###一、使用git管理项目源码
1、本地新建目录，进入新建目录右键打开git bash 
2、初始化git init
###二、配置用户信息（适用于团队协作使用区分用户）
1、git config --global user.name "用户名" (配置用户名)
2、git config --global user.email "邮箱" (配置用户邮箱)
###三、上传代码（存储到.git仓库中）
1.git add ./readme.md (添加上传文件，add（添加）)
  git add ./  (./添加所有文件)
2.git commit -m "说明信息" (添加说明信息,commit(提交))

###四、错误操作说明
1.如果提交命令时 git commit -m "说明信息"，-m忘记输入会进入另一个界面只需要按esc键 输入 :q!(强制退出)

###五、查看代码有无放到暂存区
1.git status（status：状态）

###六、提交所有修改过的文件
1.git commit --all -m "提交所有修改文件"  （--all所有）
