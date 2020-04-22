## /bin/bash^M: 坏的解释器: 没有那个文件或目录
### 错误原因
这个文件在Windows 下编辑过，在Windows下每一行结尾是\n\r，而Linux下则是\n，所以才会有 多出来的\r。
### 解决方案
使用指令`sed -i 's/\r$//' xxxxxxx.sh`，上面的指令会把 xxxxxxx.sh 中的\r 替换成空白！
