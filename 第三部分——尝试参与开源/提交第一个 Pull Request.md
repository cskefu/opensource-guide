###  尝试参与开源：提交第一个 Pull Request

####  什么是 Pull Request

​		这个是由 GitHub 提出的概念。根据 GitHub 的官方文档，Pull Request 是一种通知机制，它可以告知仓库的其他开发者，你推送了一个仓库新分支。 通过Pull Request ，你可以和仓库的协作者一起讨论和审查提交的代码，审查通过后，就可以提交到仓库的主分支中。

​		Pull Request 本质上是一种协同工作的机制，可以进行基于网络的多人提交，审核机制，审核通过后，就可以合并到主分支中。

####  提交 Pull Request 的步骤

​		第一步，你需要 fork 别人的仓库。也就是复制别人的仓库到你自己的仓库中。

​		第二步，在你自己的仓库上，修改然后提交之后，在网页端点击"New pull request"按钮。

​		在接下来的网页上有 base 仓库和 head 仓库，其中 base 是你想要提交的仓库，head 分支是你已经提交变更的仓库。

​		第三步，在提交中，描述提交本地提交的说明。


#### 实际操作一下

1. 在 GitHub 上建立两个帐号A和B。

1. 使用 A 帐号，创建项目 pull_request_demo
   
1. 在本地提交 README.md
   ```
   echo "# " >> README.md
   git init
   git add README.md
   git commit -m "first commit"
   git branch -M main
   git remote add origin https://github.com/A/pull_request_demo.git
   git push -u origin main
   ```

1. 使用 B 帐号登录 GitHub，然后fork 该项目。

1. 下载项目到本地

   ```
   git clone https://github.com/B/pull_request_demo
   echo "# add form B" >> README.md
   git add README.md
   git commit -m "modify "
   git push
   ```

1. 使用 B 帐号登录 GitHub，进入 pull_request_demo 仓库，点击 Pull request 链接。

1. 使用 B 帐号登录 GitHub，进入 pull_request_demo 仓库，点击 Pull request 链接。

1. 选择 base 和 head 仓库。点击 "New pull request"按钮。

1. 填写提交说明后，"Create pull request"

1. 使用 A 帐号登录 GitHub，进行 pull_request_demo 项目。

1. 可以看到 Pull request 中有新的数据

1. 点击 Confirm merge，完成合并。

