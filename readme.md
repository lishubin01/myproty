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

###六、提交所有修改过的文件到房间（版本库）
1.git commit --all -m "提交所有修改文件"  （--all所有）


###七、查看提交日志记录
1.git log  （查看所有提交信息）
  git log --oneline  （在一行显示一条数据）


###八、回退到指定版本
1.git reset --hard Heade~0 (回退到第一个版本)

###九、创建分支
注：主要用于团队协作时提交不完整功能时不会影响别的用户使用
1.git branch dev (说明：创建了一个分支名为dev的分支，主分支默认是master)

###十、查看当前有哪些分支
1.git branch

###十一、从默认主分支marster切换到创建的分支
1.git checkout dev  （切换到创建的子分支为dev，checkout:切换）

###十二、从创建的子分支回到默认主分支master
1.git checkout master

###十三、合并分支
1.git merge dev  （把当前分支与指定分支（dev）合并，merge：合并）
注1：当前分支指的是“git branch” 命令有星号（*）的分支；
注2：合并分支时如果有冲突需要手动处理

###十四、删除分支
1.git branch -d dev  (删除一个分支为dev的分支)

###十五、上传代码到GitHub上
1.git push [地址] master
实例：“git push git@github.com:lishubin01/myproty.git master”
说明：会把当前分支上传到远程的master分支上；
注：如果是第一次使用需要输入github的账号和密码；

###十六、从GitHub上面拉取代码到本地
1.git pull [地址] 分支名（master）
注：本地要初始化一个仓储；

###十七、从GitHub上面克隆代码到本地
1.git clone [地址]
说明：clone和pull一样，一般用pull，pull会做相应的合并，而clone多次使用会覆盖本地内容
例子：“git clone git@github.com:lishubin01/myproty.git”

###十八、添加ssh
1.ssh-keygen -t rsa -C "lishubinlife@163.com"
说明：使用ssh公钥和私钥便于团队开发时不用提供账号和密码


###十九、push和pull
说明：先git pull [名称] master在使用git push [名称] master

###二十、push和pull简写方式
1.git remote（远程的） add  [变量名]  master（分支名）
 说明：添加一个远程仓库地址
 例：git remote  add  rogin master
2.git pull [变量名] master(分支)
  git push [变量名] master(分支)
3.git push [变量名] -u master(分支)
  说明：加上-u参数，下次push时只需要执行git push就能上传代码了（加上-u之后git会把当前分支与远程指定的分支进行关联，下次操作时只需要git push和git pull进行上传和拉取）


补充：clear（清屏）
