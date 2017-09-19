# java基础语法

一个Java程序可以认为是一系列对象的集合，而这些对象通过调用彼此的方法来协同工作。

   ·对象：对象是类的一个实例，有状态和行为。例如：一条狗是一个对象，它的状态有：颜色，名字，品种；行为有：摇尾巴，叫，吃等。
   
   ·类：类是一个模板，它描述一类对象的行为和状态。
   
   ·方法：方法就是行为，一个类可以有很多方法。逻辑运算，数据修改以及所有动作都是在方法中完成的。
   
   ·实例变量：每个对象都有独特的实例变量，对象的状态有这些实例变量的值决定。
   
# 编写Java程序时，应注意一下几点：

    ·大小写敏感：Java是大小写敏感的，这就意味着标识符Hello与hello是不同的。
    
    ·类名：对于所有的类来说，类名的首字母应该大写，如果类名由若干个单词组成，那么每个单词的首字母应该大写，例如：MyFirstJavaClass
    
    ·方法名：所有的方法名都应该以小写字母开头。如果方法名含有若干单词，则后面的每个单词首字母大写。
    
    ·源文件名：源文件名必须和类名相同。当保存文件的时候，应该使用类名作为文件名保存（切记Java是大小写敏感的），文件名的后缀为.java
    
    ·主方法入口：所有的Java程序由public static void main(String[] args)方法开始执行。
   
# Java标识符：

Java所有的组成部分都需要名字。类名，变量名以及方法名都被称为标识符。

关于Java标识符，有以下几点需要注意：

    ·所有的标识符都应该以字母（A-Z或者a-z），美元符（$）,或者下划线（——）开始。
    
    ·首字符之后可以是字母（A-Z或者a-z），美元符（$）,或者下划线（——）或者数字的任何字符组合。
    
    ·关键字不能用作标识符。
    
    ·标识符是大小写敏感的
    
    ·合法标识符举例：age ，$salary,_value_,_1_value
    
    ·非法标识符举例：123abc , -salary
    
 # Java修饰符
 
 像其他语言一样，Java可以使用修饰符来修饰类中方法和属性。主要有两类修饰符：
    
    ·访问控制修饰符：default，public，protected，private
    
    ·非访问控制修饰符：final，abstract，strictfp
    
 # Java变量
 
 Java中主要有如下几种类型的变量：
 
    ·局部变量
    
    ·类变量（静态变量）
    
    ·成员变量（非静态变量）
    
# Java数组
    
数组是储存在堆上的对象，可以保存多个同类型变量。

# Java枚举

Java5.0引入了枚举，枚举限制变量只能是预先设定好的值。使用枚举可以减少代码中的bug。

例如，我们为果汁店设计一个程序，它将限制果汁为小杯，中杯，大杯。这就意味着它不允许顾客点除了这三种尺寸外的果汁。

示例：

class FreshJuice {
   enum FreshJuiceSize{ SMALL, MEDIUM , LARGE }
   FreshJuiceSize size;
}
 
public class FreshJuiceTest {
   public static void main(String []args){
      FreshJuice juice = new FreshJuice();
      juice.size = FreshJuice.FreshJuiceSize.MEDIUM  ;
   }
}
    
    
