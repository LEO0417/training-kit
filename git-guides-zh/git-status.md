# Git Status

```sh
git status
```

`git status` 显示你的 Git 工作目录和暂存区的当前状态。

## `git status` 的作用是什么？

有疑问时，运行 `git status`。这总是一个好主意。`git status` 命令只输出信息，它不会修改本地仓库中的提交或更改。

`git status` 的一个有用特性是，它会根据你的当前情况提供有用的信息。一般来说，你可以指望它告诉你：

- `HEAD` 指向哪里，无论是分支还是提交（这是你"检出"到的地方）
- 你当前目录中是否有任何尚未提交的更改文件
- 更改的文件是否已暂存
- 如果你当前的本地分支链接到远程分支，那么 `git status` 会告诉你你的本地分支是否落后或领先于任何提交

在合并冲突期间，`git status` 还会确切地告诉你哪些文件是冲突的来源。

## 如何使用 `git status`

### `git status` 的常见用法和选项

- `git status`：最常用于其默认形式，这显示了一个良好的基本信息基础
- `git status -s`：以短格式给出输出
- `git status -v`：显示更"详细"的细节，包括任何未提交文件的文本更改

你可以在 [git-scm 的文档](https://git-scm.com/docs/git-status) 中查看 `git status` 的所有选项。

## 相关术语

- `git clone [url]`：克隆（下载）GitHub 上已存在的仓库，包括所有文件、分支和提交。
- `git remote -v`：显示关联的远程仓库及其存储的名称，如 `origin`。
- `git remote add origin <url>`：添加远程，以便你可以在新初始化的仓库中与他人协作。
- `git push`：将所有本地分支提交上传到远程。
- `git push -u origin main`：首次推送分支时，这种类型的推送将配置远程和本地仓库之间的关系，以便你将来可以使用 `git pull` 和 `git push` 而不需要额外的选项。 