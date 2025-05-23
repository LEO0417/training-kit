# Git Push

```sh
git push
```

`git push` 将所有本地分支提交上传到相应的远程分支。

## `git push` 的作用是什么？

`git push` 使用本地提交更新远程分支。它是 Git 中四个与远程仓库交互的命令之一。你也可以将 `git push` 视为更新或发布。

默认情况下，`git push` 只更新远程上的相应分支。因此，如果你在执行 `git push` 时检出到 `main` 分支，那么只有 `main` 分支会被更新。在推送到远程之前，使用 `git status` 查看你在哪个分支上总是一个好主意。

## 如何使用 `git push`

在本地进行更改并提交后，你可以使用 `git push` 将它们与远程仓库共享。将更改推送到远程使你的提交对可能与你协作的其他人可访问。这还将更新你正在处理的分支的任何打开的拉取请求。

作为最佳实践，在将任何新更改推送到远程分支之前，运行 `git pull` 命令很重要。这将使用其他贡献者可能已推送到远程的任何新更改更新你的本地分支。在推送之前拉取可以减少你在 GitHub 上创建的合并冲突数量 - 允许你在将更改推送到远程分支之前在本地解决它们。

### `git push` 的常见用法和选项

* `git push -f`：强制推送否则会被阻止的推送，通常是因为它将删除或覆盖现有提交（谨慎使用！）
* `git push -u origin [分支]`：在推送新分支时很有用，这会创建一个与你的本地分支有持久关系的上游跟踪分支
* `git push --all`：推送所有分支
* `git push --tags`：发布尚未在远程仓库中的标签

你可以在 [git-scm 的文档](https://git-scm.com/docs/git-push) 中查看 `git push` 的所有选项。

## 为什么我不能推送？

如果你尝试 `git push` 但遇到问题，有一些常见的解决方案。

### 检查你的分支

使用 `git status` 检查你当前在哪个分支上。如果你在受保护的分支（如 `main`）上工作，你可能无法直接将提交推送到远程。如果这发生在你身上，没关系！你可以通过几种方式解决这个问题。

#### 工作尚未在任何分支上

1. 从当前提交创建并检出到新分支：`git checkout -b [分支名]`
2. 然后，将新分支推送到远程：`git push -u origin [分支名]`

#### 意外提交到错误的分支

1. 检出到你打算提交到的分支：`git checkout [分支名]`
2. 合并你确实意外提交到的分支的提交：`git merge [main]`
3. 将你的更改推送到远程：`git push`
4. 通过检出到该分支，找到它应该指向的提交，并使用 `git reset --hard` 来纠正分支指针，修复其他分支

## 相关术语

- `git commit -m "描述性消息"`：在版本历史中永久记录文件快照。
- `git clone [url]`：克隆（下载）GitHub 上已存在的仓库，包括所有文件、分支和提交。
- `git status`：总是个好主意，这个命令显示你在哪个分支上，工作区或暂存区中有哪些文件，以及其他重要信息。
- `git pull`：使用 GitHub 上相应远程分支的所有新提交更新当前本地工作分支。`git pull` 是 `git fetch` 和 `git merge` 的组合。 