==在新类中调用窗体控件==：https://www.cnblogs.com/marvelousone/p/7305468.html
 
==ComboBox====下拉列表框宽度自适应==：https://blog.csdn.net/weixin_42378319/article/details/118670075
 
==计时==：Stopwatch 先调用 Start 方法，然后调用 Stop 方法，最后使用 Elapsed 属性或者使用 ElapsedMilliseconds 属性得到运行时间（这两个属性的区别是前者得到的是TimeSpan实例，后者得到的是毫秒）。使用 IsRunning 可以确定 Stopwatch 的当前状态是正在运行还是已经停止。每次调用 Start 时开始累计运行时间计数；每次调用 Stop 时结束当前时间间隔测量，并冻结累计运行时间值。 使用 Reset 方法可以清除现有 Stopwatch 实例中的累计运行时间。+ [https://blog.csdn.net/zls365365/article/details/128887745](https://blog.csdn.net/zls365365/article/details/128887745) + [https://www.cnblogs.com/vaevvaev/p/6929967.html](https://www.cnblogs.com/vaevvaev/p/6929967.html)
 
==dataGridView==指定列排序：1、https://www.cnblogs.com/dotnet261010/p/6828380.html  
2、https://www.cnblogs.com/gy725/archive/2011/09/08/2171532.html  
滚动条置顶：dataGridView1.FirstDisplayedScrollingRowIndex = dataGridView1.Rows[0].Index;//滚动条置顶  
获取列名：https://blog.csdn.net/qingkaqingka/article/details/87617215  
交换行：https://www.coder.work/article/1589152  
==DataTable====任意两行交换位置：==https://www.cnblogs.com/swtool/p/5246645.html  
日期列排序（仅供参考，未测试）：https://blog.csdn.net/weixin_30457065/article/details/96576104
   

==休眠：==#include \<sys/wait.h\>  
举例:  
sleep(1);   休眠一秒  
usleep(1000);   休眠一毫秒  
usleep(1000*1000);   休眠一秒
 
==c#== ==Winform== ==保====存上一次窗体关闭时的文本（链接====1====的第五步改为链接====2====的第二步，链接====2====的第三步看情况写，可不写）==：1、https://blog.csdn.net/weixin_44077524/article/details/106903917  
2、https://blog.csdn.net/qq_52170996/article/details/119106416
 
==c# Winform====判断文本框是否为空：==https://jingyan.baidu.com/article/49711c6122aba4ba441b7cbc.html
 
c#报错：==线程间操作无效====:== ==从不是创建控件====“====button1====”====的线程访问它。==  
原代码：button1.Text = "搜索";  
不报错代码：https://blog.csdn.net/sy95122/article/details/110071147  
this.BeginInvoke((EventHandler)delegate  
{  
button1.Text = "搜索";  
});  
或者  
this.Invoke(new EventHandler(delegate  
{  
label6.Text = (int.Parse(label6.Text) +1).ToString();  
}));
   

listbox控件允许复制：https://q.cnblogs.com/q/48636/  
listbox控件允许多行选中：https://blog.csdn.net/zunguitiancheng/article/details/123188138