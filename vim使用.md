# Vim 使用

## 学习路径

	- 数字+命令: 无论什么命令都可重复数字次
	## 移动命令
	- 行内移动: w,b,0,$,^:跳到
	- 行数移动: gg, G, 3gg, 3G
	- 屏幕移动: Ctrl+b, + f, H,M,L
	- 段落移动：[, ] :以空格划分段落
	- % [匹配成对{的括号}之间光标]
	- 标记与回去
	- m[aA-zZ], '[aA-zZ]
	## 选中命令 
	- 选中文本【visual mode】 
	- v, V, C-v
	- visual mode 可以和移动模式连用: gg, G, v3ggd
	## 编辑命令
	- 撤销&反撤销：u & ctrl+r
	- 删除文本：x, d, 3dd, D:一致删除到行尾
	- 删除命令配合移动命令:
	- 例1：删掉这六个字.
	- 至少3办法：diw, vex , df.
	- 例2：删掉这六行.
	- delete row 1 
	- delete row 1 
	- delete row 1 
	- delete row 1 
	- delete row 1 
	- delete row 1 
	- Vjjjjx, ma标记之后，d'a
	## 复制粘贴 
	- y(移动命令)
	- 3yy
	- p
	- 
	- 例子1: 复制粘贴这4行
u cant see me
u cant see me
u cant see me
u cant see me
	- 方法1: Vjjj p
	- 方法2: 4yy p
	- 方法3: 先标记ma再y'a
	- 例子2: 空行连续复制粘贴5次

        - yy5p
	- 例子2: 空行连续复制粘贴5次
	## 替换
	- r, R:替换行光标后的字符
	- 例子3: 连续替换掉这行文本 
	## 索排
	- >>, <<, .
	- 例子1: 缩放这行代码
			- 例子2:缩放这行代码,并且利用上.
	- 例子3: 多行代码统一缩进
	- 例子3: 多行代码统一缩进
	- 例子3: 多行代码统一缩进
	- 例子3: 多行代码统一缩进
	- 答案：只需要Vjjj>统一缩进,然后按.重复即可
	## 查找
	- /, n, N
	- 取消高亮：再查找一个没见过的
	- 单词快速匹配: *, 然后*，#上下移动
	## 查找替换
	- :%s/被替换/要替换/gc: 固定格式
	- y, n, a, q, 
	- 例子4: python 改为 world
	- hello python 
	- 以上是全局替换，还有范围内替换
	- 先选中，然后再:s///gc
	- 例子5: python python go go d, 三个go替换成空格
	## 插入命令
	o, O, i, I, a, A
	## 编辑命令配合数字
	例6 连续输入*********** 10个型号
	-********** 
	-10i*Esc....
	## 利用visual模式 给多行代码加注释
	"print('u r an ...')
	"print('u r an ...')
	"print('u r an ...')
	"print('u r an ...')
	"print('u r an ...')
	"print('u r an ...')
	"print('u r an ...')

	## 命令行模式扩展
	- :e hello.py 如果本命令没有保存，不允许进入edit 模式
	- :e. :打开目录 
	- :n new 新建文件
	- :w 文件名：另存为
	
	## 分屏命令
	- :sp
	- :vsp
	- ctrl+w hjkl
	- ctrl+w w: 切换窗口
	- ctrl+w r: 窗口互换·
	- ctrl+w c: close
	- ctrl+w o: close other
	- ctrl+w q: close 当前
	 
## 快捷使用
 	- 单个tab内 各种分屏


