init the pr flow

## 添加新的a功能，和a.js文件

## 添加新的b功能，和b.js文件

整个流程
1. clone仓库到本地
2. 创建自己的开发分支 `git checkout -b feat/add-a`
3. 写代码之后提交 `git add .    git commit -m "feat: 创建新的功能a"`
4. 把本地仓库提交到远程仓库，把本地的feat/add-a分支提交到远程仓库 `git push origin feat/add-a`
5. 再github中提交pr
6. 想要继续开发新的功能，切换到main分支，然后更新main分支代码 `git checkout main      git pull origin main`

为什么会出现pr错误呢
1. 当两个人同时拉取main分支到自己本地，在自己的本地中开发代码，但是如果两个人修改了同一行a代码之后，第一个人提交没有问题，第二个人pr的时候就会报错，因为两个人同时修改了a，但是第二个人提交的晚就会报错。
2. 解决方法，第二个人不修改a代码，或者重新拉取main分支到自己重新修改代码。
