# 一些可能用到的vim命令，方便使用

vim自带的帮助文档，可以学习很多命令，进入vim编辑器命令模式，输入[:help],看帮助文档


hjkl  左下上右 (一般使用方向键就行)
w  光标移动到下一词  
b  与w反向  
ctrl ]  进入当前光标下的tag  
ctrl o  返回，与ctrl ]相反, jump list  
ctrl t  返回，tag stack  
crtl f  下翻页,光标移动到页顶 (就记住可用 pgup 与 pgdn 上下翻页键)  
ctrl b  上翻页,光标移动到页底
ctrl d  下翻半页，光标位置不对
ctrl u  上翻半页
ctrl e  下翻一行，光标行不变
ctrl y  上翻一行，光标行不变
zz 光标行置于中间，光标行不变  ZZ 保存并退出vim
zt 光标行置于顶，光标行不变
zb 光标行置于底，光标行不变

x  删一个字符
3x 删除3个字符，数字理解为3倍的x命令效果
dd 删除一行
3dd  删除光标处三行
dw 删除一个词
u  撤销
ctrl r  redo,反撤销  
U  撤销行修改，按两次，redo  
J  下一行合并到光标行，自动加空格  
i 进入编辑模式，光标在字符前面  
a 进入编辑模式，光标在字符后面  
$ 光标到行尾   (可以用 home 与end 方便在行收尾切换)  
^ 光标到非空字符行首  
gg 光标到文件首行头  
G  光标到文件尾行头  
o  新建下一行，进入下一行编辑  
O  新建上一行，进入上一行编辑  


y 复制  
yw 复制词，光标所在到词尾间的词  
3yw 复制3个词  
p 粘贴  
3p 粘贴三次  

3gg  去行号3  
:4   去第四行，最后要回车执行  
4G   去第四行  
2j   向下两行  

ge  光标到上一个词的词尾  
0   行首  
home键  行首  
end键   行尾  

/normal   查找字符串normal  
n  上面的查找后，n可以直接查找下一个  
N  查找后，N与n反向查找  

:set mouse=a  使用鼠标滚动页面，而不是移动光标，点击定位光标
:set mouse-=a 关闭鼠标

crtl v 开始列编辑选择

:set showcmd 显示normal模式输入的命令

vim -p one.txt two.txt  多文件tab窗口编辑
gt   切换到下一个tab窗口
2gt  切换到低2个tab窗口
:qa! 退出全部tab
:wqa 保存

"ay  复制到a寄存器，寄存器是["a]
"ap  粘贴a寄存器内容

:make target   编译makefile
:cw   当编译出现问题时显示errorlist window, 移动到报错显示的文件行上，enter进入文件窗口编辑
ctrl ww  errorlist wondow与编辑窗口切换



