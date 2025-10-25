/*
如何获取一个随机数
1.可以使用java提供的API：Math类的random()
2.random（）调用以后会返回一个[0.0,1.0）范围内的double型随机数

3.需求1：获取一个[0,100]范围内的随机整数？
   需求2：获取一个[1,100]范围内的随机整数？

4.需求：获取一个[a,b]范围的随机整数？
  (int)(Math.random()*(b-a+1))+a
*/

class RandomTest
{
 	public static void main(String[] args)
	{
		double d1=Math.random();
		System.out.println("d1="+d1);

		int num1=(int)(Math.random()*101);  //[0.0,1.0）--> [0.0,101.0) --> [0,100]
		System.out.println("num1="+num1);

		int num2=(int)(Math.random()*100)+1;  //[0.0,1.0）--> [1.0,100.0) --> [1,100]

	}
}