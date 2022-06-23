# os-lab1-syscall
OS-LAB-SYSCALL-EXTENSION

### exec.c
实现一个系统调用，使其返回后不再发生页故障。
sys_execve对可执行文件的代码和数据实现的是**需求加载**，在执行时才将其从磁盘加载到内存，此时会发生页故障
sys_execve2在系统调用返回前，仿照do_no_page的行为，为代码和数据分配页帧，将其立即加载到内存中

### getdents.c
实现一个系统调用，遍历目录中的目录项，将其写到linux_dirent结构体指针中

### sleep.c
实现一个系统调用，使当前进程睡眠相应的时间（单位 $$s$$）

### getcwd.c
实现一个系统调用，获取当前的工作路径
