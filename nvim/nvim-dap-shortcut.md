## debug
- 以C语言文件为例，假设现有文件test.c,先将文件编译为可以debug的版本
```clang --debug test.c -o test```

- 设置开始断点
  - <leader>db
- 设置结束断点
  - <leader>db

- 开始进入debug模式
  - <leader>dr 输入test.c已经编译好的文件test,就可以开始调试了
