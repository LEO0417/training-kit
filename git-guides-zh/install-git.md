# 安装 Git

如何在任何操作系统上安装 Git

Git 可以安装在最常见的操作系统上，如 Windows、Mac 和 Linux。事实上，Git 默认安装在大多数 Mac 和 Linux 机器上！

## 检查 Git

要查看你是否已经安装了 Git，打开你的终端应用程序。

- 如果你在 Mac 上，寻找一个名为"Terminal"的命令提示符应用程序。
- 如果你在 Windows 机器上，打开 Windows 命令提示符或"Git Bash"。

一旦你打开了终端应用程序，输入 `git version`。输出将告诉你安装了哪个版本的 Git，或者它会提醒你 `git` 是一个未知命令。如果它是一个未知命令，请继续阅读并找出如何安装 Git。

## 使用 GitHub Desktop 安装 Git

安装 GitHub Desktop 也会安装最新版本的 Git（如果你还没有安装的话）。使用 GitHub Desktop，你可以获得一个带有强大 GUI 的 Git 命令行版本。无论你是否安装了 Git，GitHub Desktop 都提供了一个简单的 Git 协作工具。你可以[在这里了解更多](https://desktop.github.com/)。

## 在 Windows 上安装 Git

1. 导航到最新的 [Git for Windows 安装程序](https://gitforwindows.org/) 并下载最新版本。
2. 一旦安装程序启动，按照 **Git Setup** 向导屏幕中提供的说明操作，直到安装完成。
3. 打开 Windows 命令提示符（或 **Git Bash**，如果你在 Git 安装期间选择不使用标准 Git Windows 命令提示符）。
4. 输入 `git version` 以验证 Git 是否已安装。

注意：[`git-scm`](https://git-scm.com/download/win) 是下载 Windows 版 Git 的流行和推荐资源。从 `git-scm` 下载 Git 的优势是你的下载自动开始于包含推荐命令提示符 `Git Bash` 的最新版本 Git。下载源与上述步骤中引用的 [Git for Windows 安装程序](https://gitforwindows.org/) 相同。

## 通过 Visual Studio Code 在 Windows 上安装 Git

GitHub 集成通过 [GitHub Pull Requests and Issues 扩展](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) 提供。
要开始在 VS Code 中使用 GitHub，你需要创建一个账户并安装 GitHub Pull Requests and Issues 扩展。
一旦你安装了 [GitHub Pull Requests and Issues 扩展](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)，你需要登录。按照提示使用 GitHub 进行身份验证并返回 VS Code。

---

注意：你可以执行操作，例如，你可以使用命令面板（Ctrl+Shift+P）中的 Git: Clone 命令或使用源代码管理视图中的 Clone Repository 按钮（当你没有打开文件夹时可用）从 GitHub 搜索和克隆仓库。
[在这里了解更多](https://code.visualstudio.com/docs/editor/github)

---

## 在 Mac 上安装 Git

大多数版本的 MacOS 已经安装了 `Git`，你可以通过终端使用 `git version` 激活它。但是，如果由于某种原因你没有安装 Git，你可以使用以下几种流行方法之一安装最新版本的 Git：

### 从安装程序安装 Git

1. 导航到最新的 [macOS Git 安装程序](https://sourceforge.net/projects/git-osx-installer/files/git-2.23.0-intel-universal-mavericks.dmg/download?use_mirror=autoselect) 并下载最新版本。
2. 一旦安装程序启动，按照提供的说明操作，直到安装完成。
3. 打开命令提示符"terminal"并输入 `git version` 以验证 Git 是否已安装。

注意：[`git-scm`](https://git-scm.com/download/mac) 是在 Mac 上下载 Git 的流行和推荐资源。从 `git-scm` 下载 Git 的优势是你的下载自动开始于最新版本的 Git。下载源与上述步骤中引用的 [macOS Git 安装程序](https://sourceforge.net/projects/git-osx-installer/files/git-2.23.0-intel-universal-mavericks.dmg/download?use_mirror=autoselect) 相同。

### 从 Homebrew 安装 Git

[Homebrew](https://brew.sh/) 是 macOS 的流行包管理器。如果你已经安装了 Homebrew，你可以按照以下步骤安装 Git：

1. 打开终端窗口并使用以下命令安装 Git：`brew install git`。
2. 一旦命令输出完成，你可以通过输入 `git version` 来验证安装。

## 在 Linux 上安装 Git

有趣的事实：Git 最初是为了版本控制 Linux 操作系统而开发的！所以，它很容易配置在 Linux 上运行是有道理的。

你可以通过你的发行版附带的包管理工具安装 `Git`。

### Debian/Ubuntu

1. Git 包可以使用 `apt` 获得。
2. 确保你运行的是最新版本是个好主意。为此，导航到你的命令提示符 shell 并运行以下命令以确保一切都是最新的：`sudo apt-get update`。
3. 要安装 Git，运行以下命令：`sudo apt-get install git-all`。
4. 一旦命令输出完成，你可以通过输入 `git version` 来验证安装。

### Fedora

1. Git 包可以使用 `dnf` 获得。
2. 要安装 Git，导航到你的命令提示符 shell 并运行以下命令：`sudo dnf install git-all`。
3. 一旦命令输出完成，你可以通过输入 `git version` 来验证安装。

注意：你可以在 [git-scm 的文档](https://git-scm.com/download/linux) 中下载适当的 Git 版本并阅读更多关于如何在特定 Linux 系统上安装的信息，如在 Ubuntu 或 Fedora 上安装 Git。

## 安装 Git 的其他方法

想要通过源代码安装 Git？[在这里了解更多](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)。 