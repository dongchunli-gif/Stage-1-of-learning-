/*
小岳参加考试，他和老岳达成承诺
如果：
成绩为满分100分，送跑车
(80,99]，送自行车
[60，80]，环球一日游
其他，挨揍
*/

class IFElseTest1{
 	public static void main(String[] args){

		int score =61;

		if(score==100){
			System.out.println("跑车");
		}
		else if (score>80 && score<=99){
			System.out.println("自行车");
		}
		else if(score>=60 && score<=80){
			System.out.println("环球一日游");
		}
		else{
			System.out.println("挨揍");
		}
	}
}