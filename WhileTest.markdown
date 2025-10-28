/*
循环结构之一：while循环

1.凡是循环结构，就一定会有四个要素
①初始化条件
②循环条件 ---> 一定是boolean类型的变量或者表达式
③循环体
④迭代条件

2.while的格式
①
while(②){
       ③
       ④
}

3.执行过程：① - ② - ③ - ④ - ② - ③ - ④ - ... - ②

4.for循环与while循环可以相互转换

5.for和while循环的小区别：初始化条件的作用域范围不同，while循环中的初始化条件在while循环结束后，依然有效
*/
class WhileTest
{
 	public static void main(String[] args)
	{	
		//需求1：遍历50词hello world
		int i=1;
		while(i<=50){
			System.out.println("Hello,World!");
			i++;//千万不能忘记
		}
		//需求2：遍历1-100以内的偶数，并获取偶数的个数，获取所有偶数的和
		int j=1;
		int count =0;
		int sum =0;
		while(j<=100){
			if(j%2==0){
				System.out.println(j);
				count ++;
				sum+=j;
			}
			j++;
		}
		System.out.println("偶数的个数为："+count);
		System.out.println("偶数的总和为："+sum);

	}
}