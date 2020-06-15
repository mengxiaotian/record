# 命令快捷键  

## 终端快捷键  

### 编辑命令  

Ctrl + a ：移到命令行首  
Ctrl + e ：移到命令行尾  
Ctrl + f ：按字符前移（右向）  
Ctrl + b ：按字符后移（左向）  
Alt + f ：按单词前移（右向）  
Alt + b ：按单词后移（左向）  
Ctrl + xx：在命令行首和光标之间移动  
Ctrl + u ：从光标处删除至命令行首  
Ctrl + k ：从光标处删除至命令行尾  
Ctrl + w ：从光标处删除至字首  
Alt + d ：从光标处删除至字尾  
Ctrl + d ：删除光标处的字符  
Ctrl + h ：删除光标前的字符  
Ctrl + y ：粘贴至光标后  
Alt + c ：从光标处更改为首字母大写的单词  
Alt + u ：从光标处更改为全部大写的单词  
Alt + l ：从光标处更改为全部小写的单词  
Ctrl + t ：交换光标处和之前的字符  
Alt + t ：交换光标处和之前的单词  
Alt + Backspace：与 Ctrl + w ~~相同~~类似，分隔符有些差别 [感谢 rezilla 指正]  

### 重新执行命令  

Ctrl + r：逆向搜索命令历史  
Ctrl + g：从历史搜索模式退出  
Ctrl + p：历史中的上一条命令  
Ctrl + n：历史中的下一条命令  
Alt + .：使用上一条命令的最后一个参数  

### 控制命令  

Ctrl + l：清屏  
Ctrl + o：执行当前命令，并选择上一条命令  
Ctrl + s：阻止屏幕输出  
Ctrl + q：允许屏幕输出  
Ctrl + c：终止命令  
Ctrl + z：挂起命令  

### Bang (!) 命令  

!!：执行上一条命令  
!blah：执行最近的以 blah 开头的命令，如 !ls  
!blah:p：仅打印输出，而不执行  
!$：上一条命令的最后一个参数，与 Alt + . 相同  
!$:p：打印输出 !$ 的内容  
!*：上一条命令的所有参数  
!*:p：打印输出 !* 的内容  
^blah：删除上一条命令中的 blah  
^blah^foo：将上一条命令中的 blah 替换为 foo  
^blah^foo^：将上一条命令中所有的 blah 都替换为 foo  


## tmux快捷键  

### 系统指令。  

前缀	指令	描述  
Ctrl+b	?	显示快捷键帮助文档  
Ctrl+b	d	断开当前会话  
Ctrl+b	D	选择要断开的会话  
Ctrl+b	Ctrl+z	挂起当前会话  
Ctrl+b	r	强制重载当前会话  
Ctrl+b	s	显示会话列表用于选择并切换  
Ctrl+b	:	进入命令行模式，此时可直接输入ls等命令  
Ctrl+b	[	进入复制模式，按q退出  
Ctrl+b	]	粘贴复制模式中复制的文本  
Ctrl+b	~	列出提示信息缓存  

### 窗口（window）指令。  

前缀	指令	描述  
Ctrl+b	c	新建窗口  
Ctrl+b	&	关闭当前窗口（关闭前需输入y or n确认）  
Ctrl+b	0~9	切换到指定窗口  
Ctrl+b	p	切换到上一窗口  
Ctrl+b	n	切换到下一窗口  
Ctrl+b	w	打开窗口列表，用于且切换窗口  
Ctrl+b	,	重命名当前窗口  
Ctrl+b	.	修改当前窗口编号（适用于窗口重新排序）  
Ctrl+b	f	快速定位到窗口（输入关键字匹配窗口名称）  

### 面板（pane）指令。  

前缀	指令	描述  
Ctrl+b	"	当前面板上下一分为二，下侧新建面板  
Ctrl+b	%	当前面板左右一分为二，右侧新建面板  
Ctrl+b	x	关闭当前面板（关闭前需输入y or n确认）  
Ctrl+b	z	最大化当前面板，再重复一次按键后恢复正常（v1.8版本新增）  
Ctrl+b	!	将当前面板移动到新的窗口打开（原窗口中存在两个及以上面板有效）  
Ctrl+b	;	切换到最后一次使用的面板  
Ctrl+b	q	显示面板编号，在编号消失前输入对应的数字可切换到相应的面板  
Ctrl+b	{	向前置换当前面板  
Ctrl+b	}	向后置换当前面板  
Ctrl+b	Ctrl+o	顺时针旋转当前窗口中的所有面板  
Ctrl+b	方向键	移动光标切换面板  
Ctrl+b	o	选择下一面板  
Ctrl+b	空格键	在自带的面板布局中循环切换  
Ctrl+b	Alt+方向键	以5个单元格为单位调整当前面板边缘  
Ctrl+b	Ctrl+方向键	以1个单元格为单位调整当前面板边缘（Mac下被系统快捷键覆盖）  
Ctrl+b	t	显示时钟  

## vimmium 快捷键  

### 导航当页  

?       显示help，查询vimium的所有使用方法  
h       向左滚动  
j       向下滚动  
k       向上滚动  
l       向右滚动  
gg      滚动到顶部  
G       滚动到底部  
d       向下滚动半页  
u       向上滚动半页面  
f       显示链接字母，在当前页面打开  
F       显示链接字母，在新的页面打开  
r       刷新  
gs      显示网页源代码  
i       进入插入模式，所有按键的命令都无效，直至ESC键退出  
yy      将当前的网址复制到剪贴板  
yf      显示链接字母，并将网址拷贝到剪贴板  
gf      cycle forward to the next frame  
gF      focus the main/top frame  

### 打开新的页面  

o       搜索网址，书签，或历史记录，在当前页面打开  
O       搜索网址，书签，或历史记录，在新的页面打开  
b       搜索书签，在当前页面打开  
B       搜索书签，在新的页面打开  

### 代码查找  

/       进入查找模式，输入关键字查找，ESC退出  
n       切换到下一个匹配  
N       切换到上一个匹配  

### 前进后退  

H       后退  
L       前进  

### 切换tab  

J, gT   切换到左边tab  
K, gt   切换到右边tab  
g0      切换到第一个tab  
g$      切换到最后一个tab  
^       切换到刚才的tab  
t       创建一个新的页面  
yt      复制当前页面  
x       关闭当前页面  
X       恢复刚才关闭的页面  
T       在当前所有的tab页面中搜索  
<a-p>   pin/unpin current tab  

### 标记  

ma      当页标记，只能在当前tab页面跳转，m + 一个小写字母  
mA      全局标记，可以再切换到其他tab的跳转过来，m + 一个大写字母  
`a      跳转到当页标记  
`A      跳转到全局标记  
``      跳回之前的位置  

### 控制命令  

]], [[  Follow the link labeled 'next' or '>' ('previous' or '<')  
          - helpful for browsing paginated sites  
<a-f>   open multiple links in a new tab  
gi      focus the first (or n-th) text input box on the page  
gu      跳转到当前网址的上一级网址  
gU      跳转到当前网址的跟网址  
ge      编辑当前的网址，在当前页面打开  
gE      编辑当前网址，在新的页面打开  
zH      滚动到最左边  
zL      滚动到最右边  
v       enter visual mode; use p/P to paste-and-go, use y to yank  
V       enter visual line mode  

### 其他  

5t      数字num + t，打开num个tab页面  
<Esc>   ESC按钮，可以从任意控制命令中退出，也可以从任意模式中退出（例如插入模式、查找模式）  


