简单介绍用法：https://www.cnblogs.com/52php/p/5840229.html  
示例2：https://blog.csdn.net/ShenHang_/article/details/106674378  
删除：unlink(路径名);
 
设置超时select函数介绍：https://www.cnblogs.com/wuyepeng/p/9745573.html  
用例参考（注意参考中FD_SET(0,&reads)中0是标准输入fd，改为要监控的fd（open文件时获取），且无返回值；select(1,&temps,0,0,&timeout)处1应为fd+1）：https://blog.csdn.net/asdaqqwc/article/details/108736687
 
脚本非阻塞fifo：https://www.jianshu.com/p/ddef1d209f1c  
脚本操作参看（用处不大）：https://blog.csdn.net/m0_43405302/article/details/121590045