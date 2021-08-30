# Git

 1.设置全局的用户名和邮箱，每次提交的时候的信息

```DOS
git config --global user.email "181356288@qq.com"
git config --global user.name "Doman"
```

2.生成ssh登录公钥和私钥

``` 
ssh-keygen -t rsa -C "181356288@qq.com"
```

3.存储地点

```
ssh-keygen -t rsa -f  D:\Github  -C "test key"

-t 指定密钥类型，默认是 rsa ，可以省略。
-C 设置注释文字，比如邮箱。
-f 指定密钥文件存储文件名。

1.确认秘钥的保存路径（如果不需要改路径则直接回车）；
2. 如果上一步置顶的保存路径下已经有秘钥文件，则需要确认是否覆盖（如果之前的秘钥不再需要则直接回车覆盖，如需要则手动拷贝到其他目录后再覆盖）；
3.创建密码（如果不需要密码则直接回车）；（该密码是你push文件的时候要输入的密码，而不是github管理者的密码）
当然，你也可以不输入密码，直接按回车。那么push的时候就不需要输入密码，直接提交到github上了
这里我们选择按回车不输出密码
4. 确认密码；
```

4.初始化仓库（在笔记文件夹目录下）

```DOS
git init  
```

5.提交所有变化（一旦修改status就会改变）

```
git add -A  

其他命令：
git add -u  提交被修改(modified)和被删除(deleted)文件，不包括新文件(new)
git add .  提交新文件(new)和被修改(modified)文件，不包括被删除(deleted)文件6.
```

6.查看是否已经追踪

```
git status
```

7.提交，并生成上传的注释

```
git commit -m "XXXXX"

git commit命令，-m后面输入的是本次提交的说明
```

8.将本地库版本推送到 github 中

```
git push git push origin master git@github.com:dj181356288/notebook.git
```

