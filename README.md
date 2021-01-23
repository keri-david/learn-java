# keri自学java日记
这是keri从2021/1/22建立的仓库，用来记录寒假自学java语言的过程，计划一天一提交，直到开学为止。  
目前在学慕课上的java零基础课程：[链接](https://www.icourse163.org/learn/ZJU-1001541001?tid=1450243457#/learn/announce)
## ***Day1:***
- java的初学者ide是eclipse,本人使用archlinux,安装方法为yay -S eclipse-jee,java环境为openjdk-8,Mac和Windows从官网可下载java和ide；
- 用eclipse去写第一个java程序——helloWorld，新建项目之后，右击src文件夹，新建class类，勾选下面第一个[public......]选项，目前作用不知，以后知道的话会记录；
- ide的自动补全，不会自己跳出来，需要你去按下ALT+/，之后上下选择，回车确定，System.out.println("helloWorld");用println是输出后自动换行，点击上面绿色播放按钮编译运行软件，可以事先按下CTRL+S保存下，之后console栏会输出结果；
- helloworld完成，我们学习java的输入，Scanner in = new Scaner（System.in），注意当你补全Scanner时要注意选择util相关的那个，随后会自动生成import java.util.Scanner；之后我们可以看下输入的内容有没有被读取到，System.out.println（“echo：” + in.nextLine（））；返回的内容就是echo：加上你输入的内容；
- 选择多行的操作，按下SHIFT的同时按方向键；多行加注释的方法，选中多行后，按CTRL+/，去掉注释也是同样的按键；
- 接下来看下System.out.println（2+3+“=2+3=”+（2+3））；的结果是?	5=2+3=5	这就是计算优先级所导致的，注意后面的2+3如果不加括号，那么就是23；
- 赋值操作：int price=0；price=in.nextInt（）；同样如果输入是一个浮点型就用nextFloat（）；in作为一个读取工具可以多次赋值，比如int price=0,count=0；price=in.nextInt（）；count=in.nextInt（）；在console栏可以输入一个之后按空格、回车、制表键等，第一个输入的数字就被赋值到了price,第二个到了count，in在使用完毕后要close掉；
- java 定义常量： final int amount=100；之后不能更改；
- 整型和整型运算，结果只有整型，是不完整的，只要有一个变量是浮点型，那么结果也是浮点型，比如12变成12.0；整型变量赋值给浮点型变量不会出现问题，而浮点型便来嗯赋值给整型变量就要做强制转换，并且会有数据丢失；
- 浮点数运算有误差，因为浮点数在存储时的复杂方法，我们一般用整型运算。
- 单目运算的优先级最高（是指只有一个算子的运算，比如正号和负号），赋值的优先级最低，他们的运算顺序都是从左往右；（乘除、取余）和(加减、字符窜连接的“+”）依次；

## ***Day2:***
- 关系运算就不记录了，所有编程语言都通用，运算级较低，但是比赋值高，其中==和！=优先级比其他运算更低，运算顺序从左往右；
- 判断两个浮点数是否相等，用两个数的差值的绝对值是否小于一个很小的数字，比如：Math.abs（a-b）< 1e-6；
- 条件判断语句，如果只有一句执行语句，那么可以不要大括号；
- 设置断点，用debug模式；双击一行的左侧，出现蓝色点，然后点击那个虫子，就是debug模式，按下F6一行一行执行，按下右上角的java布局，回到正常编辑模式；
- else总是和最近的if匹配；可以用大括号逻辑上分割开；
- 如果else if过多，可以用switch-case：switch（a）{case 1：。。。；case 2：。。。default：。。。}，break跳出匹配；
- 常见错误：
|两行以上执行语句，没有加大括号；|
|if后面直接加了分号，导致大括号内容无关判断语句一直都执行；|
|判等时，只用一个=；|

## ***Day3:***			
