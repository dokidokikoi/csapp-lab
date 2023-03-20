# csapp-lab
csapp lab

### datalab
使用64位环境编译32位程序很有可能出现如下错误提示：
```
/usr/bin/ld: 当搜索用于 /usr/lib/gcc/x86_64-redhat-linux/4.8.5/libgcc_s.so 时跳过不兼容的 -lgcc_s
```
以及
```
/usr/include/gnu/stubs.h:7:27: fatal error: gnu/stubs-32.h: No such file or directory
```

我们需要安装两个包：
```bash
$ sudo yum install -y glibc-devel.i686 libstdc++-devel.i686
```
