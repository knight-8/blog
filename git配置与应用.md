<!--
 * @Author: your name
 * @Date: 2022-03-11 13:30:27
 * @LastEditTime: 2022-03-14 00:34:45
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \blog\git配置.md
-->
如何在github创建一个仓库并连接本地git

（1）创建仓库，连接ssh
（2）配置git，依次运行下列命令
git config --global user.name 你的英文名
git config --global user.email 你的邮箱
git config --global push.defaul matching
git config --global core.quotepath false
git config --global core.editor "vim"
配置完成
（3）将本地仓库上传至远程github
git remote add origin github地址
git push -u origin 分支名

git命令
git init 初始化本地仓库，在目录里创建一个.git目录
git status -sb 显示当前所有文件状态
-s是summary总结 -b是branch分支
git add 文件名 : 添加，把文件变动放在git暂存区
git commit -m "xxx" : 提交所有变动给.git仓库
git log 查看变更历史


将本地仓库变动上传至GitHub
git pull 拉取github变动
git push 将所有变动推送至github
git clone github地址 下载远程仓库