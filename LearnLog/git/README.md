# LearnLog

## Simple description per commit

- 2021/06/19 16:54:23 ==primary learning log document add==

  - MyGithubOverview.md

  - git initial step:

    ```
    create a new repository on the command line
    
    echo "# LearnLog" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M master
    git remote add origin https://github.com/tataerduoha1/LearnLog.git
    git push -u origin master
    ```

- 2021/06/19 22:53:18 ==Plan doc added & GithubOverview doc modified==

  - add plan dirs to log every step

  - git push

    ```
    git push -u origin master
    ```

  - git 添加dev分支 参考 [Github创建新分支](https://www.jianshu.com/p/4b95058088c2)

    - git branch 查看本地分支

    - git branch -r 查看远程分支

    - git branch -a 查看所有分支

    - git branch dev 本地创建dev分支

    - git checkout dev 切换到新分支

      ```
      git checkout -b dev
      
      <==>
      
      git branch dev
      ```

    git checkout dev

    ```
    - git push origin dev 推送dev新分支到github# LearnLog
    ```

  - git 上传无需账号密码设置[Linux 上传代码到github](https://www.cnblogs.com/siyuan1998/p/10720420.html)

    - ```
      ssh-keygen -t rsa -C "注册Github用的邮箱" ##本地生成密钥
      cd ~/.ssh 
      cat id_rsa.pub ##获取秘钥，内容全部复制
      
      ##github操作方法：GitHub主页==>settings==>SSH and GPG keys==>New SSH Key==>title随意填写，key填写之前id_rsa.pub全部内容==>Add SSH key
      
      ##运行 ssh -T git@github.com
      1.输入 yes 回车
      2.然后如果你看到 Permission denied (publickey). 就说明你失败了，请回到第 1 步重来，是的，回到第 1步重来；如果你看到 Hi xxx! You've successfully authenticated, but GitHub does not provide shell access.
      
      ## 之后即可轻松使用，无需输入账号密码
      ```