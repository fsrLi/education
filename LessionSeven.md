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

  ***休息一下,练习试试：<br/>***
  ![休息一下](https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fc-ssl.duitang.com%2Fuploads%2Fitem%2F202003%2F12%2F20200312172704_LmVey.thumb.400_0.jpeg&refer=http%3A%2F%2Fc-ssl.duitang.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1689470625&t=40b06035a20603c23a7425dd291814d1)

### liunx中的文本搜索指令
  ***简单的文本处理时使用grep:<br>***
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

  ***复杂自定义文本处理时使用awk（如果客户的要求不到万不得已不要使用awk）<br/>***
  1.基本语法<br/>
    `awk 'pattern { action }' input_file`<br/>
      ·pattern是匹配条件<br/>
      ·action是满足条件时的动作<br/>
      ·input_file是输入文件<br/>

  2.打印文件所有内容<br/>
    `awk '{ print }' input_file`<br/>
    思考：这和上面哪个指令的效果一样？<br/>
    思考：<br/>
  ![思考](https://hbimg.huabanimg.com/43aeaa5474db9c7862ffb444c6f758802dced7ad30e73-AusXpJ_fw658)

  3.使用自定义字符过滤：<br/>
    `awk -F',' -v OFS=':' '{ print $1, $NF }' test.txt`<br/>
    作用：使用冒号(:)作为输入字段分隔符，并将输出字段分隔符设置为逗号(,)，然后打印每行的第一个字段和最后一个字段。<br/>

  4.根据条件筛选结果<br/>
    `awk '{ if ($1 > 60) print "good"; else print "bad" }' test.txt`<br/>

  ※awk提供了丰富的筛选及匹配选项供大家使用，这里只是举个栗子，剩下的有待大家自己开发

### 管道符
    `|`<br/>
    管道符作为连接使用，将该符号的前面指令的输出作为输入进入后面的指令<br/>

### 定时任务
  1.查看当前所有定时任务<br/>
  `crontab -l`<br/>
  2.写入定时任务<br/>
  `crontab -e`<br/>
  3.定时任务构成<br/>
    `minute hour day month day_of_week command_to_run`<br/>
     ·minute            第几分(0-59)<br/>
     ·hour              第几小时(0-23)<br/>
     ·day               第几天(1-31)<br/>
     ·month             第几个月(1-12)<br/>
     ·day_of_week       一周的第几天(0-7，其中0和7都表示星期日)<br/>
     ·command_to_run    执行命令<br/>
