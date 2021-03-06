# Git 和 Github 是什么
### Git是一个分布式版本管理系统
举个例子就是一篇文章大家共同写作，一起修改，Git就是帮你记录谁怎么改了，最终应该合并成什么样子。
### Github是一个远程仓库网站
大家在本地上有自己的代码仓库和版本管理，但想要和别人协作则需要一个远程的仓库，别人直接访问你的远程仓库作为你发布的稳定的版本
> PS：[这里有廖雪峰的git教程](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/)
# Git工作流程
以两个人开发为例，其中一个人为主要负责人，另外一位为参与工作者。 
1. 主要负责人的远程仓库为项目的仓库，参与者在GitHub上fork主要负责人的远程仓库（也就是拷贝一份）作为参与者自己的远程仓库。
2. 参与者从自己的远程仓库下载代码到自己本地，作为本地仓库。
3. 参与者在本地开发，修改代码，完成后[提交](http://www.runoob.com/git/git-basic-operations.html)给本地的Git。
4. 参与者完成本地提交后，将本地仓库代码推送到自己的远程仓库。
5. 参与者推送到自己远程仓库后，在GitHub上进行pull request，请求让项目仓库来拉取参与者的远程仓库的代码更新。
6. 负责人审核要拉取的内容，审核通过就融合代码，不通过就关闭请求。
7. 当负责人更新了项目仓库后，参与者需要先[添加项目仓库作为本地仓库的远程仓库之一](http://www.cnblogs.com/chucklu/p/4056373.html)（只有拉取权限），将项目仓库的更新和自己本地代码融合后，再更新自己的远程仓库，以保持一致。
> PS: 关于冲突 当你执行pull操作后git提示不能自动merge融合代码时会在相应的本地文件上标注出冲突的部分，将代码改成你需要的部分后把标注删掉，再在本地上添加和提交即可。
