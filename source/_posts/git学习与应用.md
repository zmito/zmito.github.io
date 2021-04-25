---
title: git学习与应用

date: 2021-04-24 20:36:34

tags: git密钥

---

---------------------
* 密钥的生成  指定密钥名


```bash

ssh-keygen -t rsa -C email@email.com -f ~/.ssh/gitee

```
---------------------------
* 修改或新建 .ssh/config  文件

```
Host gitee.com
    IdentityFile ~/.ssh/gitee  ##指定密钥文件

```
--------------------------------------------------------

#### -----       重要：必须将公钥添加到远程仓库站点的 用户设置 ssh 

* gitee.com 用户设置中添加 ssh 公钥:  ~/.ssh/gitee.pub 内容

--------
* 测试链接
``` 
ssh -T git@gitee.com

```
-------------------------
* 一个项目推送到多个远程仓库

```bash

git remote add gitee git@gitee.com  ## 添加要推送到的远程仓库地址及指定别名

git push -u gitee master            ## 推送到指定别名的远程对应的分支

```
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          
                                                                                                                                                                                                                                                                                                                          