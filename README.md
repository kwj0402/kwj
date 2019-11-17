# kwj
实验名称：字符串实验


实验目的：掌握字符串String及其方法的使用
                掌握异常处理结构


要求：内容: 利用已学的字符串处理知识编程完成 《长恨歌》 古诗的整理对齐工作， 写出 
功能函数，并运行。达到如下功能: 

1. 每 7 个汉字加入一个标点符号， 奇数时加“，” 偶数时加".” 。
2.允许提供输入参数，统计古诗中某个字或词出现的次数 。
3.考虑操作中可能出现的异常，在程序中设计异常处理程序。


核心代码：    StringBuffer u=new StringBuffer(“汉皇重色思倾国御宇多年求不得……”);//创建字符串1
                    StringBuffer u1=new StringBuffer("不");//创建字符串2
                    for (int i = 7;i<u.length();i+=8) {
	        u.insert(i, "，");
	            }
	    for (int a = 15;a<u.length();a+=15) {
	        u.deleteCharAt(a);
	            }
	    for (int b = 15;b<u.length();b+=16) {
	        u.insert(b, "。");
	            }
	    for (int c = 16;c<u.length();c+=17) {
	        u.insert(c, "\n");//用for循环插入标点符号“，”和“。”
	            }

boolean b=u.toString().contains(u1);//寻找此子字符串是否被包含在此字符串之中

System.out.println("包含次数为："+count(u.toString(),u1.toString()));//调用count，输出包含次数

static int count(String s1,String s2)//统计子字符串被包含次数

while((index=s1.indexOf(s2,index))>-1)//indexOf查找字符串的第一次出现

运行截图：


编程感想：这次编程对我而言难度中等偏上，主要是奇数和偶数位置插入不同的符号有点难度。运用for循环成功的解决了。让我对JAVA有了更好的感觉。我相信在老师的带领下我会继续进步。
