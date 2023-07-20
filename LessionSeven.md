# Liunx
## 什么是liunx
  是一种免费使用和自由传播的类UNIX操作系统,简单理解为和windows一样的操作系统即可

## liunx与batch的关系
### 什么是batch
  batch也叫作批处理，指的是非图形化界面/可视化界面的程序处理

### 为什么batch处理需要使用liunx
  1.文本为主导:liunx本身即为文件控制，也可以说liunx是一种特殊的文本构成系统（windows中有很多dll等无法看见的编译文件，但liunx的系统文件可以理解为全部都是文本文件）,正因为如此，liunx在处理文本信息时更加的高效便捷，短板为用户化界面。
  2.命令行工具和脚本的强大生态系统：Linux操作系统自带丰富的命令行工具和实用程序，这些工具可以用于各种任务，从文件处理到网络操作。这种强大的工具生态系统为编写复杂的批处理脚本提供了更多的可能性。
  3.开源：liunx的系统是完全开放的，可以根据需要随意改写系统，这也就方便了一些特殊的batch处理

## 初始Liunx
### liunx的界面
  1.图形界面<br>
  2.命令行界面<br>
  ※需要大家掌握的是命令行界面<br>
  举个栗子：<br/>
  ![举个栗子](https://img.ixintu.com/download/jpg/202001/2e6ec91cbd78b42e39ae3e92556b99d4.jpg!con)

### liunx中的基本命令
  1.显示用户：<br>
    `who am i`<br>
  2.显示当前路径：<br>
    `pwd`<br>
  3.显示当前路径下所有文件：<br>
    `ls`<br>
  4.显示当前路径下所有文件的权限：<br>
    `ls -l`<br>
    `ll`<br>
  5.创建文件夹
    `mkdir`<br>
  6.创建文件
    `touch`
  7.修改权限：<br>
    `chmod`<br>
  8.编辑文件内容：<br>
    `vi`<br>
  9.显示文件内容：<br>
    `cat`<br>
  10.帮助指令<br/>
     `man`<br/>
  11.历史输入<br/>
     `history`<br/>
  举个栗子：<br/>
  ![举个栗子](https://img.ixintu.com/download/jpg/202001/2e6ec91cbd78b42e39ae3e92556b99d4.jpg!con)

  休息一下,练习试试：<br/>
  ![休息一下](https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fc-ssl.duitang.com%2Fuploads%2Fitem%2F202003%2F12%2F20200312172704_LmVey.thumb.400_0.jpeg&refer=http%3A%2F%2Fc-ssl.duitang.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1689470625&t=40b06035a20603c23a7425dd291814d1)

### liunx中的文本搜索指令
### grep
    1.基本搜索<br/>
      `grep keyWord File`<br/>
    2.忽略大小写<br/>
      `grep -i keyWord File`<br/>
    3.显示行号<br/>
       `grep -n keyWord File`<br/>
    4.递归搜索<br/>
        `grep -r keyWord Dirctory/`<br/>
    5.正则表达式搜索<br/>
        `grep -E keyWord File`<br/>

### awk
    1.基本语法<br/>
      awk 'pattern { action }' input_file<br/>




    
