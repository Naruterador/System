## Vim 分屏编辑
#### 基本指令
```shell 
#水平分割窗口，同时打开file1和file2
vim -o file1 file2

#垂直分割窗口，同时打开file1和file2
vim -O file1 file2:

#关闭当前窗口
Ctrl+W c

#关闭当前窗口，如果只剩最后一个了，则退出Vim
Ctrl+W q

#把光标移到下一个的屏中
Ctrl+W w
```

#### 分屏
```shell
上下分割当前打开的文件
Ctrl+W s

上下分割，并打开一个新的文件
:sp filename

左右分割当前打开的文件
Ctrl+W v

左右分割，并打开一个新的文件
:vsp filename
```

#### 移动光标
```shell
把光标移到右边的屏
Ctrl+W l

把光标移到左边的屏中
Ctrl+W h

把光标移到上边的屏中
Ctrl+W k

把光标移到下边的屏中
Ctrl+W j

把光标移到下一个的屏中
Ctrl+W w
```

#### 移动分屏
```shell
向右移动
Ctrl+W L

向左移动
Ctrl+W H

向上移动
Ctrl+W K

向下移动
Ctrl+W J
```

#### 水平分割 
```shell    
#把当前窗水平分割成两个窗口。Ctrl-w s快捷键可以将当前窗口进行水平分割
:split(:sp)  

#水平分割窗口，并在新窗口中显示另一个文件
:split filename  

#水平分割出一个n行高的窗口
:nsplit(:nsp)  

#水平分割出一个n行高的窗口，并编辑一个新文件。 (Ctrl-w n或 Ctrl-w Ctrl-n)
:[n]new  

#水平分割出一个窗口，并在新窗口打开名称为光标所在词的文件 
Ctrl+w f 

#水平分割一个窗口，打开刚才编辑的文件
Ctrl-w Ctrl-^
```

#### 垂直分割
```shell
#把当前窗口分割成水平分布的两个窗口。 (Ctrl-w v或Ctrl-w Ctrl-v)
:vsplit(:vsp)  

#垂直分割出一个新窗口
:[n]vne[w]  

#水平分割的命令 
:vertical

#垂直分割指令
:horizontal
```

#### 关闭子窗口
```shell
#关闭所有窗口，退出vim
:qall  

#保存所有修改过的窗口
:wall

:only  

#关闭当前窗口，Ctrl-w c能实现同样的功能。 (象 :q :x同样工作 )
:close  
```

#### 调整窗口大小
```shell
#当前窗口增高一行。也可以用n增高n行
Ctrl+w + 

#当前窗口减小一行。也可以用n减小n行
Ctrl+w - 

#当前窗口扩展到尽可能的大。也可以用n设定行数
Ctrl+w _ 

#当前窗口n行高
:resize n 

#所有窗口同样高度
Ctrl+w =  

#当前窗口的高度设定为n行
n Ctrl+w _  

#当前窗口减少一列。也可以用n减少n列
Ctrl+w < 

#当前窗口增宽一列。也可以用n增宽n列
Ctrl+w > 

#当前窗口尽可能的宽。也可以用n设定列数
Ctrl+w | 
```

#### 在vim下打开终端
```shell
:term
```

