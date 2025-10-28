/*
循环结构之一：do-while循环

1.凡是循环结构，就一定会有四个要素
①初始化条件
②循环条件 ---> 一定是boolean类型的变量或者表达式
③循环体
④迭代条件

2.do-while的格式
①
do{
     ③
     ④
}while(②);

执行过程：① - ③ - ④ - ② - ③ - ④ - ... - ②

3.说明：
1)do-while循环至少执行一次循环体
2)for、while、do-while循环三者之间是可以相互转换的。
3)do-while循环结构，在开发中，相较于for、while循环来讲，使用的较少。

*/

class DoWhileTest
{
 	public static void main(String[] args)
	{
		//需求：遍历100以内的偶数，并输出偶数的个数和总和
		int i=1;
		int count=0;
		int sum=0;
		do{
			if(i%2==0){
				System.out.println(i);
				count ++;
				sum+=i;
			}
			i++;
		}while(i<=100);
		System.out.println("偶数的个数为："+count);
		System.out.println("偶数的总和为："+sum);


	}
}