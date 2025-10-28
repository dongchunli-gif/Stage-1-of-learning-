/*
分支结构之switch-case的使用

1.语法格式
switch（表达式）{

	case 常量1：
		//执行语句1
		//break;
	case 常量2：
		//执行语句2
		//break;
	....
	default:
		//执行语句2
		//break;


}

2.执行过程：
根据表达式中的值，依次匹配case语句，一旦与某一个case中的常量相等，那么就执行此case中的执行语句。
执行完此执行语句之后，
		情况1：遇到break，则执行break后，跳出当前的switch-case结构
		情况2：没有遇到break，则继续执行其后的case语句。  ---->case穿透
		...
		直到遇到break或者执行完所有case及default中的语句，退出当前的switch-case结构
3.说明：
①switch中 的表达类型只能式特定的数据类型，如下：byte / short / char / int / 枚举 / String（jdk7.0新增）
②case后都是跟的常量，使用表达式与这些常量做相等的判断，不能进行范围的判断
③开发中，使用switch-case时，通常case匹配的情况都有限。
④break：可以使用在switch-case结构中。一旦使用此break关键字，就跳出当前的switch-case结构
⑤default：类似于if-else中的else结构。default是可选的，而且位置是灵活的。


4.switch-case与if-else之间的转换
①开发中凡是能使用swith-case结构的场景都能转化为if-case，反之，不成立
②开发中，如果一个具体问题既可以使用switch-case，又可以使用if-case的时候，推荐使用switch-case
   为什么？因为switch-case效率较高。
*/
import java.util.Scanner;
class SwitchCaseTest
{
 	public static void main(String[] args)
	{
		Scanner scanner =new Scanner(System.in);
		int num=scanner.nextInt();
		switch(num){
			case 0:
				System.out.println("zero");
				break;
			case 1:
				System.out.println("one");
				break; //结束当前switch-case结构
			case 2:
				System.out.println("two");
				break;
			case 3:
				System.out.println("three");
				break;
			default:
				System.out.println("other");
				break;
				}
		
	}
}