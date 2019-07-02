# LearnGit
学习Git的使用
mac 学习Git使用
1, 打开终端: 输入git,  若出现以下信息,则证明安装过git 
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
[--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
[-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
[--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
<command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
clone      Clone a repository into a new directory
init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
add        Add file contents to the index
mv         Move or rename a file, a directory, or a symlink
reset      Reset current HEAD to the specified state
rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
bisect     Use binary search to find the commit that introduced a bug
grep       Print lines matching a pattern
log        Show commit logs
show       Show various types of objects
status     Show the working tree status

grow, mark and tweak your common history
branch     List, create, or delete branches
checkout   Switch branches or restore working tree files
commit     Record changes to the repository
diff       Show changes between commits, commit and working tree, etc
merge      Join two or more development histories together
rebase     Reapply commits on top of another base tip
tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
fetch      Download objects and refs from another repository
pull       Fetch from and integrate with another repository or a local branch
push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.

2, 若没有git的信息 , 建议用homebrew安装git , 具体方法自行查询,这里不做过多描述
3,配置git信息: 
git config --global user.name "你的username"
git config --global user.email "你的邮箱地址"
4,配置完成之后,通过终端命令创建 ssh key : ssh-keygen -t rsa -C "你的邮箱地址"
5, 我们这使用默认的一路回车就行。成功的话会在~/下生成.ssh文件夹，进去，打开id_rsa.pub，复制里面的key(注意如果找不到路径, 执行: defaults write com.apple.finder AppleShowAllFiles -bool true因为有些隐藏的文件不显示)
6,终端查看 open.ssh/id_rsa.pub
7,回车后: cat.ssh/id_rsa.pub
8,复制rsa开头的key
9,登录GitHub,添加ssh key 点击settings,如图: ICON下的图1,
10,然后添加ssh key : 图2
11,终端输入 ssh -T git@github.com 进行连接的验证:
Hi wangy0925! You've successfully authenticated, but GitHub does not provide shell access.表示连接成功
12,提交本地项目到GitHub  图三
13, 填写项目信息, 图四
14,Clone工程到本地,首先复制ssh地址
15, 打开终端,把工程克隆在桌面, git clone  Github地址

6)提交修改，首先切换到LearnGit文件路径：

cd /Users/jamesruio/Desktop/LearnGit

然后输入:

//文件添加到仓库（.代表提交所有文件）

git add .

//把文件提交到仓库

git commit -m "First Commit"

//上传到github 








