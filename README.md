# gdb-helper
一款利用调用api来辅助gdb使用的工具
## 安装
如果是sys贯通课程的学生，可以直接运行setup.sh
随后将gdb.sh中的.gdbinit的路径设置正确，.gdbinit中设置.api_key的路径，最好都放在project目录下
## 如何使用
大部分用法参考[gdb dashboard](https://github.com/cyrus-and/gdb-dashboard)

**特殊用法**
### 1.gh
用`gh` 加要求来获取命令提示，按回车接受，随便按一个键加回车拒绝
如
`gh 断在printk`
`gh 断在stvec`

### 2.whatis
whatis，简称wi，随后加寄存器或者某一个想问的位，如
`whatis sepc`
`wi mstatus`
`wi mideleg`
`whatis SSIP`
**这里采用数据库构造，数据库的数据由大模型清洗处理，可能存在问题，中文翻译可能不准确，有问题欢迎提交issue与PR**

