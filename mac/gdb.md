# gdb


### 常用命令
```
1.  回车键：重复上一命令
2. （gdb）help：查看命令帮助，具体命令查询在gdb中输入help + 命令,简写h
3. （gdb）run：重新开始运行文件（run-text：加载文本文件，run-bin：加载二进制文件）,简写r
4. （gdb）start：单步执行，运行程序，停在第一执行语句
5. （gdb）list：查看原代码（list-n,从第n行开始查看代码。list+ 函数名：查看具体函数）,简写l
6. （gdb）set：设置变量的值
7. （gdb）next：单步调试（逐过程，函数直接执行）,简写n
8. （gdb）step：单步调试（逐语句：跳入自定义函数内部执行）,简写s
9. （gdb）backtrace：查看函数的调用的栈帧和层级关系,简写bt
10.（gdb）frame：切换函数的栈帧,简写f
11.（gdb）info：查看函数内部局部变量的数值,简写i
12.（gdb）finish：结束当前函数，返回到函数调用点
13.（gdb）continue：继续运行,简写c
14.（gdb）print：打印值及地址,简写p
15.（gdb）quit：退出gdb,简写q
16.（gdb）break+num：在第num行设置断点,简写b
17.（gdb）info breakpoints：查看当前设置的所有断点
18.（gdb）delete breakpoints num：删除第num个断点,简写d
19.（gdb）display：追踪查看具体变量值
20.（gdb）undisplay：取消追踪观察变量
21.（gdb）watch：被设置观察点的变量发生修改时，打印显示
22.（gdb）i watch：显示观察点
23.（gdb）enable breakpoints：启用断点
24.（gdb）disable breakpoints：禁用断点
25.（gdb）x：查看内存x/20xw 显示20个单元，16进制，4字节每单元
26.（gdb）run argv[1] argv[2]：调试时命令行传参
27.（gdb）set follow-fork-mode child#Makefile项目管理：选择跟踪父子进程（fork()）
28. core文件：先用$ ulimit -c 1024 开启core，当程序出错会自动生成core文件。调试时 gdb a.out core
29. ctrl+c：退出输入
```