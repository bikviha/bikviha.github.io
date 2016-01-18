[Git](https://github.com/"Git") SSH key:
--------
    一 、1设置 Git 的 user name 和 email ：

>$ git config --global user.name "yourname"
>
>$ git config --global user.email "yourname@gmail.com"

    二、生成SSH密钥过程：

1. 查看是否已经有了ssh密钥：
>cd ~/.ssh

        如果没有密钥则不会有此文件夹，有则备份删除
2. 生成密钥：
>$ ssh-keygen -t rsa -C “haiyan.xu.vip@gmail.com”
>
>按3个回车，密码为空。
>
>最后得到了两个文件： id_rsa 和id_rsa.pub

    ```
Your identification has been saved in /home/tekkub/.ssh/id_rsa.
Your public key has been saved in /home/tekkub/.ssh/id_rsa.pub.
The key fingerprint is:
………………
    ```

3. 在github上添加ssh密钥，这要添加的是“`id_rsa.pub`”里面的公钥。

    ```
Titel : xxxx
Key   : (将 cat ~/id_rsa.pub 出的值，复制到此处)
    ```

***

Repositories Add
----------------
    复制一个版本库到本地 ：git Clone  git@github.com:path/name.git

基本操作流程：

    一、将 filename.txt 文件添加到本地仓库的缓存区

>   git add filename.txt

    二、给需要更新的动作，添加一个注释（实际上只是放入本地仓库的HEAD中，但是还没到你的远端仓库）

>    git commit -m "\*\*\*\*\*"

    三、将改动提交到远程仓库中

>    git push


![banner pic](/public/images/banner.jpg "banner pic")
