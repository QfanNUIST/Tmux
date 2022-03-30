# Tmux
Tmux常用操作

# 创建一个新的Tmux工作区会话
tmux new -s session_name

# 竖分屏
ctrl + b %

# 横分屏
ctrl + b "

# 新建Tmux窗口
ctrl + b c

# 切换到上/下一个窗口
ctrl + b p/n

# 切换窗格
ctrl + b o

# tmux attach命令用于重新接入某个已存在的会话。
# 使用会话编号
$ tmux attach -t 0
# 使用会话名称
$ tmux attach -t <session-name>

# tmux kill-session命令用于杀死某个会话。
# 使用会话编号
$ tmux kill-session -t 0
# 使用会话名称
$ tmux kill-session -t <session-name>

Ctrl+b %：划分左右两个窗格。
Ctrl+b "：划分上下两个窗格。
Ctrl+b <arrow key>：光标切换到其他窗格。<arrow key>是指向要切换到的窗格的方向键，比如切换到下方窗格，就按方向键↓。
Ctrl+b ;：光标切换到上一个窗格。
Ctrl+b o：光标切换到下一个窗格。
Ctrl+b {：当前窗格与上一个窗格交换位置。
Ctrl+b }：当前窗格与下一个窗格交换位置。
Ctrl+b Ctrl+o：所有窗格向前移动一个位置，第一个窗格变成最后一个窗格。
Ctrl+b Alt+o：所有窗格向后移动一个位置，最后一个窗格变成第一个窗格。
Ctrl+b x：关闭当前窗格。
Ctrl+b !：将当前窗格拆分为一个独立窗口。
Ctrl+b z：当前窗格全屏显示，再使用一次会变回原来大小。
Ctrl+b Ctrl+<arrow key>：按箭头方向调整窗格大小。
Ctrl+b q：显示窗格编号。

tmux ls命令可以查看当前所有的 Tmux 会话。
$ tmux ls
# or
$ tmux list-session



more： http://www.ruanyifeng.com/blog/2019/10/tmux.html
