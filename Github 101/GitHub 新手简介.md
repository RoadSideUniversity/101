# GitHub 新手简介

<https://medium.com/@itswisdomagain/github-101-introduction-to-github-for-newbies-efaf46c88406>

by [Arerosuoghene Wisdom](https://medium.com/@itswisdomagain)

本文是系列文章中的第二篇，旨在以更易于理解的方式解释 Git 和 GitHub。上一篇文章为新手简单介绍了 Git。如果您不熟悉 Git，请帮我们一个忙，在阅读本文之前先查看第一篇文章。只需要5分钟左右。

在上一篇文章中，我们说过您可以与朋友、同事甚至陌生人共享您的“git-tracked”文件夹（又名本地 git 存储库）。我们没有说的是 GitHub 让这一切变得非常简单。

> 哦哦。让我们暂停一下。虽然本文主要关注 GitHub，但同样的原则也适用于任何其他 git 托管平台或服务。此类其他平台/服务的示例包括 GitLab 和 Bitbucket。

好吧，我们继续。

Github 将 GitHub 定义为“用于版本控制和协作的代码托管平台。它可以让您和其他人在任何地方共同处理项目。”

够简单吗？但愿如此。但以防万一……
> GitHub 帮助您将“git-tracked”项目文件夹（又名本地 git 存储库）及其所有内容保存在云中，以便您或任何您允许的其他人可以随时随地访问它。嗯，基本上。

GitHub 和其他 git 托管平台/服务最常见的用途就是在云中保留本地 git 存储库的副本，因此，如果/当您丢失 PC 或发生其他一些事情时，您不必咬手指。

除此之外，此类平台/服务还有另一个好处——协作！能够让其他人加入您的项目，直接更改文件或审查您的工作并提出改进建议、报告错误等。在后续文章中，我们将介绍如何使用 GitHub 进行有效协作。

现在，我们来看看如何将本地存储库与 GitHub 同步。如您所知，同步是双向的。每当本地发生更改时，本地存储库就会将更新发送到远程存储库（称为推送），如果云中存在本地尚未发生的更改，您可以从远程存储库获取更新（这称为拉取）。

## GitHub 入门

前往 GitHub 并创建一个帐户 - 如果您已经有帐户，请登录。然后创建一个新项目（或存储库）。通常最好创建新项目，而无需使用 README.md 文件初始化存储库。

完成后，您将获得该项目的唯一 URL，如下所示。复制它！不，我的意思不是复制下面的 URL。复制给你的网址😉。

```
https://github.com/itswisdomagain/firebase-auth-secure-way.git
```

返回到终端/命令提示符并告诉 Git 您想要将本地存储库与 GitHub 同步。请记住在执行任何 git 命令之前在终端/命令提示符下导航到您的项目目录。将本地 git 存储库与 GitHub 托管的云存储库连接所需的命令是：

```
git remote add origin https://github.com/itswisdomagain/firebase-auth-secure-way.git
```

需要注意的事项。首先，您看到的 origin 关键字只是一个标识符。 Git 允许您将多个远程存储库连接到本地 git 设置。 Git 要求您为每个远程存储库（存储库与存储库相同）提供唯一的 ID。通常的做法是使用 origin 作为默认远程存储库的标识符。

第二个需要注意的事情应该是显而易见的，但我只是说一下。网址！该命令应以您之前复制的 URL 结尾，而不是我在该示例中使用的 URL。

