# Contributing

All contributions are welcome to this project.

## How to contribute

* **File an issue** - if you found a bug, want to request an enhancement, or want to implement something (bug fix or feature).
* **Send a pull request** - if you want to contribute code. Please be sure to file an issue first.

## Pull request 最佳实践

We want to accept your pull requests. Please follow these steps:

我们希望这样来接收你的pull requests. 请按照下面的步骤进行:

### Step 1: File an issue

Before writing any code, please file an issue stating the problem you want to solve or the feature you want to implement. This allows us to give you feedback before you spend any time writing code. There may be a known limitation that can't be addressed, or a bug that has already been fixed in a different way. The issue allows us to communicate and figure out if it's worth your time to write a bunch of code for the project.

在你写任何代码之前，请先提交一个issue描述出你想要解决或者你想要实现的feature。这会让我们在你花费时间写代码之前可以给你反馈。可能有一些已知的限制是无法定位，或者是bug但已经以其他方式修复的。issue可以让我们更好的交流和了解给这个项目写一堆代码是值得你花费时间的。

### Step 2: Fork this repository in GitHub

This will create your own copy of our repository.

这步会创建属于你自己的我们仓库的副本

### Step 3: Add the upstream source

The upstream source is the project under the Box organization on GitHub. To add an upstream source for this project, type:

upstream的源是GitHub上Box组织的那个项目。为了给当前项目增加upstream源，请键入：

```
git remote add upstream git@github.com:box/t3js.git
```

This will come in useful later.

立等可用。

### Step 4: Create a feature branch

Create a branch with a descriptive name, such as `add-search`.

创建一个见名知意的分支，比如 `add-search`.

### Step 5: Push your feature branch to your fork

As you develop code, continue to push code to your remote feature branch. Please make sure to include the issue number you're addressing in your commit message, such as:

当你开发代码的时候，继续向你的远程feature分支推送代码。请确保在你的提交消息里一定要包含你正在定位的issue号，比如：

```
git commit -m "Adding search (fixes #123)"
```

This helps us out by allowing us to track which issue your commit relates to.

这会帮助我们追踪到你的提交的代码会关联到哪个issue

Keep a separate feature branch for each issue you want to address.

请给每一个你想定位的issue创建一个独立的feature分支。


### Step 6: Rebase

Before sending a pull request, rebase against upstream, such as:

在发送pull request之前，对upstream进行rebase，如下：

```
git fetch upstream
git rebase upstream/master
```

This will add your changes on top of what's already in upstream, minimizing merge issues.

这会把你的修改置于已有upstream的头部，保证最小化合并issues

### Step 7: Run the tests

Make sure that all tests are passing before submitting a pull request.

一定要确保在提交pull request之前，所有测试都是通过的。

### Step 8: Send the pull request

Send the pull request from your feature branch to us. Be sure to include a description that lets us know what work you did.

从你的feature分支发送pull request给我们。一定要带有描述信息，它能让我们知道你做了哪些修改。

Keep in mind that we like to see one issue addressed per pull request, as this helps keep our git history clean and we can more easily track down issues.

谨记：我们喜欢看到issue对应着一个pull request，这会让我们的git历史记录干净，而且我们可以更简单的追踪问题。
