# JAVA-
BIT JAVA 정리

```java
package Pack01;

/*
// ex) 

public class Hello 
{
	public static void main(String[] args) 
	{
	}	
}
*/
```

```java
// ex1) 주석에 대한 이야기 
// 1. 화면에 숫자를 출력
// 2. 주석을 사용하는 방법
public class Hello 
{
	public static void main(String[] args) 
	{
	   // 밑의 문장은 주석문장이다.
		 // System.out.println(2000);
     // 밑의 문장은 주석이 아니다.
     // /* ~~ */ 이런식으로 전체주석을 걸어준다. 
		System.out.println(2000);
		System.out.println(3000);
		System.out.println(4000);				
	}
}

```

```java
	// ex2) 몫 과 나머지 구하는 법
 public class Hello 
{
	public static void main(String[] args) 
	{
		// 산술연산(오칙연산)
		//System.out.println(1000);
		System.out.println(17 + 3);
		System.out.println(17 - 3);
		System.out.println(17 * 3);
		System.out.println(17 / 3); // 몫
		System.out.println(17 % 3); // 나머지 
	
				// 1. 결과값 [0, 1, 2, 3, 4, 5, 6]
				// 2. 나머지가 0이 나왔을때는 7의 배수이다.	
					123456 % 7 
				// 앞에 숫자가 무엇이든지 뒤에 숫자로 나머지를 구했을때
				// 그 결과가 0이라면 뒤에 숫자의 배수이다. 
   }	

}
```

```java
// ex3)  비교연산
 public class Hello 
{
	public static void main(String[] args) 
	{
      // 비교연산 ( 대소관계연산 )
		System.out.println(true);
		System.out.println(false);
		// apple은 예약어가 아니므로 촐력 할수 없다.
		// System.out.println(apple);
		System.out.println( 10 > 5);
		System.out.println( 5 >= 5 );
		System.out.println( 5 < 3 );
		System.out.println( 5 <= 5);
		System.out.println( 5 == 4);
		System.out.println( 5 != 5);
	}
}
```

```java
//ex4) 출력 방법
public class Hello 
{
	public static void main(String[] args) 
	{
		// 숫자 출력
		System.out.println(1000);
		
		// 문자열 출력
		System.out.println("호랑이");
		
		// 숫자처럼 생긴 문자열이다.
		System.out.println("2000");
		
		// 문자열은 산술 연상이 되지 않는다.
		System.out.println("100" + "200");
		
		// 문자(1글자)를 출력한다.
		System.out.println('한');
		
	}
}
```

```java
//ex5) 숫자 와 문자열 
public class Hello 
{
	public static void main(String[] args) 
	{
		// 숫자 + 숫자 = 숫자
		System.out.println(10 + 20);
		// 숫자 + 문자열 = 문자열
		System.out.println(10 + "호랑이");
		// 문자열 + 숫자 = 문자열
		System.out.println("호랑이" + 20);
		// 문자열 + 문자열 = 문자열
		System.out.println("100" + "500");
			
		System.out.println(10 + 20 + "호랑이");
		// 결과가 호랑이30 이 아니다.
		System.out.println("호랑이" + 10 + 20);
		// 숫자 + 문자열 >> 결과가 문자열이고 + 숫자 
		System.out.println(10 + "호랑이" + 20);
		
		System.out.println(10 + " " + 20 + " " + 30);
		System.out.println("----------------------------");
		System.out.println(123456);
		
		
	}
}

```

```java
//ex6) 숫자 연산 기호 순서
public class Hello 
{
	public static void main(String[] args) 
	{
		// ( )  < 최우선
		// * , / , %  우선  
    // + , - 나중
		System.out.println( 3*4+2 ); //14
		System.out.println( 3+4*2 ); //11
		System.out.println( 3+(4*2) ); //11
		
		System.out.println( (3+4)*2 ); // 14
		System.out.println( 3 + 4 * 2 + 6); //17
		System.out.println( (3+4) * (2+6) ); //56 
		
		System.out.println( 3+(4*2) ); //11
		
	}
	
}
```

```java
//ex7) byte 의 정의
public class Hello 
{
	public static void main(String[] args) 
	{
		
		// 1byte : byte  : 8bit  : 2의 8승
		// 2byte : short : 16bit : 2의 16승
		// 4byte : int   : 32bit : 2의 32승
		// 8byte : long  : 64bit : 2의 64승
		// 컴터야 1byte 메모리 줄래.
		// byte : 타입 << 메모리를 요구하는 문자(숫자가)다르기 떄문에 타입이라 한다.
		// monkey :  변수(변수명)  << 숫자를 집어넣었을때 변할수있기 때문에 변수라 한다.
		byte monkey;
		// 변수  = ( 대입연산자 ) 
		// 변수 대입연산자 리터럴 ( 변수 대입연산자의 내용을 리터럴 ) 
		monkey = 100; // 좌 <<<<<=  우; 우측에서 좌측으로 실행된다.
		System.out.println(monkey);
		
		byte dog = 30;
		System.out.println(dog);
		// 바이트 영역 -128~ +127
		byte cat = 127;
				
		// 1byte 주세요 . >> byte
		// 2byte 주세요 . >> short
		short apple = 30000;
		System.out.println(Short.MAX_VALUE); // short의 값을 알고싶면 Short로 변경후 " . " Max_VALUE , MIN_VALUE 입력
		System.out.println(Short.MIN_VALUE);
		System.out.println(Byte.MAX_VALUE);
		System.out.println(Byte.MIN_VALUE);
		
		int banana;
		System.out.println(Integer.MAX_VALUE);
		System.out.println(Integer.MIN_VALUE);
		
		long orange;
		System.out.println(Long.MAX_VALUE);
		System.out.println(Long.MIN_VALUE);
		
		// byte ,  short , int , long 
		// 하나주세요
	}
}	
```

```java
//ex8) 변수 작명법
public class Hello 
{
	public static void main(String[] args) 
	{
		// 1. 변수이름은 중복해서 작성 할수 없다.
		int apple;
		//int apple; 이건 안된다.
		
		// 2. 대소문자는 구분이 된다.
		//    가급적 사용하지 않는것이 좋다.
		int Apple;
		
		// 3. 첫글자가 숫자가 아니라면
		//    숫자를 조합해서 사용할수 있다.
		int banana1234;
		//int 8banana; 이건 안된다.
		
		// 4. $, _ 이 두개를 제외한 특수문자를 사용할수 없다.
		int dog;
		int _dog;
		int dog$;
		//int dog#; 이건 안된다. ( '_ , $' 이거 외엔 사용 불가) 
		int _365;
		
		// 5. 한글을 변수명으로 사용할수 없다.
		//    가급적 피하는게 좋다.
		int 사과;
		사과 = 100;
		System.out.println(사과);
		
		// 6. 한단어 이상으로 변수명을 작성할때 
		// 낙타(카멜) 표기법을 사용한다.
		int applenumber; //구분이 어렵다.
		int AppleMumber; // 첫글자를 대문자로 해서 구분을 쉽게.
		int appleNumber; // 이렇게도 가능
		int rectanglearea;
		int areaOfRectangle;
	}
}
```

```java
//ex9) 원시타입 정의
public class Hello 
{
	public static void main(String[] args) 
	{
		//  1, 2, 4, 8
		// byte , short , int , long (원시타입은 총 8가지)
		// char(2byte)(한문자 , 한글자) , boolean(1byte)(ture,false)  
    // float(4byte)(소수점) , double(8byte)(소수점보다정밀)
		
		// 2byte의 메모리를 준다.
		// 문자만 전문적으로 관리하는 타입니다.
		char apple; //음수만 사용가능
		// 문법은 틀린것은 아니지만 사용방법이 틀렸다.
		apple = 20000;
		
		apple = 'A';
		System.out.println(apple);
		System.out.println((int)apple); //char 타입이지만, int를 넣음으로써 바뀐다.
		
		apple = '한';
		System.out.println(apple);
		System.out.println((int)apple);
		
		System.out.println((char)54621);
	
	   apple = 60000;
	  
			System.out.println((int)Character.MAX_VALUE);
			System.out.println((int)Character.MIN_VALUE);
	 
			   
			   // 6번째 원시타입 (Primitive)
			   boolean dog;
			   dog = true;
			   System.out.println(dog);
			   dog = false;
			   System.out.println(dog);
			   
			   // 7번쨰 ( 4byte 요청) f가 붙으면 float타입
			   float cat = 3.14f;
			   System.out.println(cat);
			   
			   // 8byte요청 f가 안붙으면 double 타입
			   double bear = 3.14;
	}
	
}
```

```java
//ex10) 변수 값
public class Hello 
{
	public static void main(String[] args) 
	{
		// 
		int a = 17;
		//
		int b;
		//
		b = 3;
		
		System.out.println(a+b);
		System.out.println(a-b);
		System.out.println(a*b);
		System.out.println(a/b);
		System.out.println(a%b);
		
		System.out.println(a > b);
		System.out.println(a != b);
		
		int c = 30, d = 40;
		System.out.println(c + "" + d);
        c = 300;
        d = 400;
        System.out.println(c + "" + d);
        
        
		
		
		
	}
}
```

```java
//ex11) num 의 정의
public class Hello 
{
	public static void main(String[] args) 
	{
		int num =  100;
		System.out.println(num);
		
		num = 200;
		System.out.println(num);
		
		num = 100 + 200; // 300
		System.out.println(num);
		
		num = num + 100 - 30; // 370
		System.out.println(num);
		
		num = num + 1; // 371
		System.out.println(num);
		
		int count = 10; 
		num = num + count * 2; // num 371 + count 20 = 391
		System.out.println(num);
		
		//int a = 10;
		//int b;
		//int c; ( 밑에와 동일한 수식어 )
		int a = 10, b, c;
		b = 20;
		c = a + b;
		System.out.println(a + "" + b + "" + c);
		
    }
}
```

```java
//ex12-1) swap 프로그램 
public class Hello 
{
	public static void main(String[] args) 
	{
		int a =  10, b = 20;
		System.out.println(a + " " + b);
		int c;
		
		c = a; // c : 10
		a = b; // a : 20
		b = c; // b : 10
		
		System.out.println(a + " " + b);
		// 교환 프로그램 또는 Swap 프로그램
	}
}

//ex12-2) 변수이름 temp
public class Hello 
{
	public static void main(String[] args) 
	{
	     int a  = 10, b = 20;
	     int t;
	     // 대각을 형성하는 조건. temp =  t
	  System.out.println(a + " " + b);  
	     t = a; // t = 10
	     a = b; // a = 20
	     b = t; // b = 10
		System.out.println(a + " " + b);
		
	}
	
}

```

```java
//ex13) 연산의 정의
public class Hello 
{
	public static void main(String[] args) 
	{
		// 산술연산 , 비교연산 , 논리연산 
		System.out.println(false || false); // false 
		System.out.println(false || true);  // true
		System.out.println(true || false);  // true
		System.out.println(true || true);   // true
		
		System.out.println("-----------------------------");
		
		System.out.println(false && false);// false
		System.out.println(false && true); // false
		System.out.println(true && false); // false
		System.out.println(true && true);  // true
		
		System.out.println("-----------------------------");
		
		System.out.println(false || true || false); // true
		
		System.out.println(false && true && false); // false
		
		System.out.println("-----------------------------");
		
		System.out.println( 3 < 2 || 10 != 10 || false);  // false
		System.out.println( 33 > 22 && 10 == 10 && true); // true
		
		System.out.println("-----------------------------");
		
		System.out.println(true && true || false); // 이렇게는 사용 하지 않는다.
		System.out.println((true && true) || false); // true
		System.out.println(true && (true || false)); // true
		
		
		int a = 10, b = 20;
		System.out.println(a < b || a*2 < b - 30);
		//System.out.println(a < b || 20 < -10); 결과값은 true
		
		// 산술 >> 비교 >> 논리 이런 순차로 실행한다.  
		System.out.println(a < b && a*2 < b - 30);
		//System.out.println(a < b && a*2 < b - 30); 결과값은 false
		
		// 논리부정연산자 ( ! 붙임으로서 부정으로 바꿈 )
		System.out.println("호랑이");
		System.out.println( !true ); // false
		System.out.println( !(3 > 2)); // false
		
		System.out.println( !( a < b && a*2 < b - 30 ) ); 
		//System.out.println( !( a < b && a*2 < b - 30 ) ); 결과값 true
		boolean gameover = true;
				System.out.println( !gameover );
				
		
	}

}

```

```java
//ex 14) if 언어의 정의
// 제어문 : if , for , while , switch
//               제어문 안에 제어문을 사용할수 있다.
//               do ( 사용해두됨 )         
public class Hello 
{
	public static void main(String[] args)
	{
		//if(){} , for(){}
		//while (){} , switch(){}
	   // (){}
		
		if( false ) // 조건을 묻는것
		{
			System.out.println(1); // 결과가 일어나지 않는다
		}
		
		if( true ) 
		{
			System.out.println(2); 
		}
	
		 System.out.println(3);
		 
		 if( 3 > 1 ) 
		 {
			 System.out.println(4); 
		 }
		 if( 3 < 1 ) 
		 {
			 System.out.println(5); 
		 }
		
		 int num = 10;
		if ( num == 10 )
			System.out.println(6);
		
		 {
			// 산술 >> 비교
			 if (num *2 == num/2 )
			 {
				 System.out.println(7);
			 }
		System.out.println("--------------------");
		int count = 24;
		if ( count / 3 == 8 )
		{
			System.out.println(8);
			if ( count % 2 == 0 ) 
			{
				System.out.println("변수 값은 짝수이다.");
			}
			System.out.println(10);
			if ( count / 10 + count % 10 == 6 )
			{
				System.out.println("호랑이");
				
			}
					System.out.println(12);
					}
				System.out.println(13);
					}
		
		}
}
```

```java
// ex 15) 짝수와 홀수 일때  if else 의 정의
public class Hello 
{
	public static void main(String[] args)
	{
		int num = 10;
		if ( num == 9 ) // 맞느냐 되물어보는 상황
		{
			System.out.println(11);
			System.out.println(12);
			System.out.println(13);
		}
		else
		{
			System.out.println(21);
			System.out.println(22);
			System.out.println(23);
		}
		System.out.println(3); 
		System.out.println("----------------------------");
		
		int count = 36;
		//짝수 일때 만족
		if( count % 2 == 0) 
		{
			int q = count / 10;  //3
			int r = count % 10;  //6
			System.out.println(q + " " + r);
			if(  q + r == 7) ;
			{
			System.out.println("호랑이");
			}
		}	
		else // 홀수인 경우
		{
		  //System.out.println("일단 숫자가 홀수임");
			if (count % 3 == 0 )
		  {
		System.out.println("변수 값은 홀수이면서 3의 배수이다.");
		  }
		else
		{
			System.out.println("변수 값은 홀수이면서 3의 배수 아니다.");
		}
			
		}
	}
}
```

```java
/ ex 16-1 ) 만족 값 찾기
public class Hello 
{
	public static void main(String[] args)
	{
		int num = 0 ; // 값이 만족했을경우 
		if( num == 0 ) 
		{
			System.out.println(0);
		}
		else if(num == 1)
		{
			System.out.println(1);
		}
		else if (num == 2)
		{
			System.out.println(2);
		}
		else
		{
			System.out.println(999);
		}
		System.out.println("호랑이");
	}
}

// ex 16-2) 
public class Hello
{
      public static void main(String[] args)
      {
    	 int jumsu = 87; // A B C D 
    	 if(jumsu >= 90)
    	 {
    		 System.out.println("A");
    	 }
    	 else if (jumsu >= 80)
    	 {
    		System.out.println("B"); 
    	 }
    	 else if (jumsu >= 70)
    	 {
        System.out.println("C");
    	 }
    	 else if (jumsu >=60)
    	 {
    		 System.out.println("D");
    	 }
    
      }
      
}
```

```java
// ex 17-1) for문 반복문의 정의
public class Hello 
{
	public static void main(String[] args) 
	{
	// for 
		// for (초기화; 조건; 증감 ) {}
		  System.out.println(" start "); 
		for (int i = 0; i <  4 ; i = i+ 1) {
					  System.out.println("호랑이");
				// for (int i = 1; i <=  100 ; i = i+ 1)
		   // 밑에 코드는 잘못된 코드
		   // for (int i = 0; i >=  4 ; i = i+ 7) 잘못된 표기
	    }
					//
					System.out.println( i + "end");
		   
			}

	}	
	

//ex 17-2) for문을 이용한 연산프로그램

public class Hello 
{
	public static void main(String[] args) 
	{
     int a  = 10;
     System.out.println(a);
     
			a= a + 2 ; // 12
     System.out.println(a);
	  
		 a = a - 7;  // 5
     System.out.println(a);
    
		 a = a + 1;  // 6
     System.out.println(a);
    
		 a++; // a = a + 1 ; 의 업그레이드된 문법
     System.out.println(a); // 7
    
		 a = 1000;
     System.out.println(a); 
    
		 a++; // 1001
     System.out.println(a);
    
		 a = a - 1; // 1000
     System.out.println(a);
    
		 a--; //  a = a + 1; 과 같은 문법
     System.out.println(a); // 999
     System.out.println("------------------------");
     
		// 5단 출력 프로그램.
     for (int i = 0; i < 10; i++) { // for문에 10으로 입력하면 10번 일어난다는 정의
		System.out.println( 5 + " * " + i + " = " + 5 * i); // 5단에 대한 연산프로그램
				}
		}	
}
```

```java
//ex 18) 합산 프로그램의 정의  sum 의 사용 의미

public class Hello 
{
	public static void main(String[] args) 
	{
	 int a = 0;
	 a = a + 1; // 1
	 a = a + 2; // 3 ( 1 + 2 )
	 a = a + 3; // 6 ( 1 + 2 + 3 )
	 a = a + 4; // 10 ( 1 + 2 + 3 + 4 )
	 a = a + 5; // 15 ( 1 + 2 + 3 + 4 + 5 )
	 System.out.println(a);
	 
	// 합산 프로그램 (sun :  합이라는 변수이름)
	 a = 0;
		for (int i = 0; i <= 5; i++) {
		a = a + i; 
	 }
		System.out.println(a);
	    
				System.out.println("------------------");
		 int sum = 0 ;
		 for (int i = 1; i <= 10; i++) {
				sum = sum + i ;
				//System.out.println(sum);
		 }
			 System.out.println("------------------");
			 System.out.println(sum);
	}	
	
}
```

```java
// ex  19) 합산 프로그램 버전업 

public class Hello 
{
	public static void main(String[] args) 
	{
	  // 단 출력 프로그램.
		int dan = 9;
		for (int i = 0; i < 10; i++) {
			System.out.println( dan + " * " + " = " + i * dan ) ;
		
		}
		System.out.println("------------------");
		
		// 합산 프로그램.
		int sum = 0;
		int num = 100;
		for (int i = 1; i <= num; i++) {
			  sum = sum + i;
			
		}
		System.out.println(sum);
		
		// 3의 4승
		//1 * 3 * 3 * 3 * 3
	
		// 승수 프로그램(거듭제곱)
		int ss = 1;
		int a1 = 2, a2 = 8;
	for (int i = 0; i < a2; i++) {
		ss = ss * a1;
	
			}
          System.out.println(ss);
	}
	
	
}
```

```java
//ex20) 제어문안에 제어문 사용 ,  이중for문

public class Hello 
{
	public static void main(String[] args) 
	{
	    for (int i = 0; i < 10; i++) {
			if( i % 2 == 0 ) 
			{
				System.out.println( i + " : even "); // 짝수
			}
			else 
			{
				System.out.println( i + " : odd "); // 홀수
			}
		}
	     
			// 이중for문
	    for (int i = 0; i < 3; i++) {
	    	System.out.println(i +"호랑이"); 
	    	for (int j = 0; j < 4; j++) {
	 			System.out.println(j +"사자");
	 	    }	
	    }
	}
	
	
}
```

```java
//ex 21) 이중for문 심화과정

public class Hello 
{
	public static void main(String[] args) 
	{
	 System.out.print("호랑이");
	 System.out.println("원숭이");
	 
	 for (int i = 0; i < 3; i++) {
		 for (int j = 0; j < 4; j++) {
			 System.out.print( "["+ i + " " + j + "]");
		}
		System.out.println();
		System.out.println();
	  }
         System.out.println("---------------");	
         
         for (int i = 0; i < 6; i++) {  // 세로
    		 for (int j = 0; j < 8; j++) {  // 가로
    			 System.out.print("* ");
       		}
    		System.out.println();
    	  }
   System.out.println("---------------");	
         
          int width = 14;
          int height = 10;
         for (int i = 0; i < height; i++) {  // 세로
    		 for (int j = 0; j < width; j++)  {  // 가로
    			 if( i == 0 || i == height-1  || j == 0 || j == width -1)  {
    				 System.out.print("* ");
    			 }else {
    				 System.out.print(". ");
    			 }
       		}
    		System.out.println();
    	  }
	}	
}
```

```java
//ex 22) char 의 정의

public class Hello 
{
	public static void main(String[] args) 
	{
	System.out.println("A");
	System.out.println('a');
	
	//char ch2 = 65;
	char ch = 'A';
	System.out.println(ch);
	// 직접 번역을 해 버린 결과이다.
	char ch2 = 65;
		System.out.println(ch2);
		
		System.out.println((char)(ch2+1));
		
	      for (int i = 0; i < 26; i++) {
		System.out.print((char)('A'+i));
		 
	      }
		System.out.println();
	   
	   for (int i = 0; i < 128; i++) {
			System.out.println((char)(i));
	 }
	}	
}

```

```java
//ex23 ) 마름모 만들기

public class Hello 

{

	public static void main(String[] args)

	{

		// ex1)

		for (int i = 0; i < 5; i++) { // 세로

			for (int j = 0; j < 5; j++) { // 가로

				System.out.print("[" + i + " " + j +"]" );

			}

			System.out.println();

		}

		System.out.println();

		

		// ex2)		

		for (int i = 0; i < 5; i++) { // 세로

			for (int j = 0; j < 5; j++) { // 가로

				int ii = i-2;

				int jj = j-2;

				

				System.out.print("[" + ii + " " + jj +"]" );

			}

			System.out.println();

		}

		System.out.println();

		

		// ex3)

		for (int i = 0; i < 5; i++) { // 세로

			for (int j = 0; j < 5; j++) { // 가로

				int ii = i-2;

				int jj = j-2;

				

				if( ii < 0 ) {

					ii = -ii; //        -(-3)

				}

				

				if( jj < 0 ) {

					jj = -jj;

				}

				System.out.print("[" + ii + " " + jj +"]" );

			}

			System.out.println();

		}

		System.out.println();

		

		// ex4)

		for (int i = 0; i < 5; i++) { // 세로

			for (int j = 0; j < 5; j++) { // 가로

				int ii = i-2;

				int jj = j-2;

				

				if( ii < 0 ) {

					ii = -ii; //        -(-3)

				}

				

				if( jj < 0 ) {

					jj = -jj;

				}

				

				if( ii+jj <= 2) {

					System.out.print("* ");

				}else {

					System.out.print("  ");

				}

			}

			System.out.println();

		}

		System.out.println();

		

		int length = 17;

		int halfLength = length / 2;

		

		// ex5)

		for (int i = 0; i < length; i++) { // 세로

			for (int j = 0; j < length; j++) { // 가로

				int ii = i-halfLength;

				int jj = j-halfLength;

				

				if( ii < 0 ) {

					ii = -ii; //        -(-3)

				}

				

				if( jj < 0 ) {

					jj = -jj;

				}

				

				if( ii+jj <= halfLength) {

					System.out.print("* ");

				}else {

					System.out.print("  ");

				}

			}

			System.out.println();

		}

		System.out.println();

	}

}

```

```java
//ex 24) switch 문장
public class Hello 
{
	public static void main(String[] args) 
	{
		// 1. switch 안에 변수를 사용할수 있다.
		// 2. case 뒤에 변수를 사용할수 없다.
		// 3. case 뒤에 오는 숫자는 중복될수 없다.
		// 4. case와 쌍으로 되는 break 를 생략하면
		//    프로그램은 계속된다. (break 를 만날때까지)
		int num = 10;
		int test = 20;
		
		switch(num) {
		case 10:
			System.out.println(1);
			//break;
		
		// case test : // 사용할수 없다.
		case 20:
			System.out.println(2);
			//break;
			
		case 30:
			System.out.println(3);
            break;
            
		default:
			System.out.println(999);
			break;
		}
		
		
		// 숫자, 문자, 문자열도 가능하다.
		switch ('한') {
		case 10:
			System.out.println(4);
			break;
		case '글':
			System.out.println(5);
			break;
		case '만':
			System.out.println(6);
		default:
			break;
		}
	
	}	
}
```

```java
//ex25) 지역변수의 개념

public class Hello 
{
	public static void main(String[] args) 
	{
		// 지역 변수 성격도 가지고
		// 전역변수의 성격도 가진다.
		int num = 10;

		{
			// 지역변수
			int apple = 20;
			System.out.println(apple);
			System.out.println();
		}
		
		System.out.println(num+10);
		//System.out.println(apple);
		
		for (int i = 0; i < 4; i++) {
			
		}
	   
		for (int i = 0; i < 4; i++) {
			
		}
		
		{
			int banana=10;
		}
	
		{
			int banana=10; // 이름을 중복으로 사용 가능
		}
	}	
}
```

```java
//ex26) switch문장 안에 for문 사용법

public class Hello 
{
	public static void main(String[] args) 
	{
			switch (10){
			case 10:{
				int sum = 0;
				for (int i =1; i <=10; i++) {
					sum = sum + i;
				}
				System.out.println(sum);
			}break;

			case 20:{
				for (int i = 0; i < 10; i++) {
					System.out.println(5 + " * " + i + " = " + 5*i);
				}
			}break;

			case 30:{
				System.out.println("호랑이");
			}break;

			default:
				break;
		}
	}	
}
```

```java
//ex 27) switch 응용법
public class Hello 
{
	public static void main(String[] args) 
	{
		//if else if else
		//switch
		int jumsu = 83;
		if(jumsu >= 90) {
			System.out.println("A");
		}else if (jumsu >= 80) {
			System.out.println("B");
		}else if (jumsu >= 70) {
			System.out.println("C");
		}else if (jumsu >= 60) {
			System.out.println("D");
		}else {
			System.out.println("F");
			
		}
		int num = jumsu / 10;
		switch (num) {
		case 10: // 읟적으로 break; 를 사용하지 않는 경우
		case 9:
			System.out.println("A");
			break;
		case 8:
			System.out.println("B");
			break;
		case 7:
			System.out.println("C");
			break;
		case 6:
			System.out.println("D");
			break;
		default:
		    System.out.println("F");
			break;
			
		}
	}	
}
```

```java
//ex 28-1) 반복문 

public class Hello 
{
	public static void main(String[] args) 
	{
		// while (){} : 반복문 : 반복 횟수를 모를때 프로그램을 작성 할때
		// for() {} : 반복문 : 반복 횟수를 알고 프로그램을 작성 할때
		int num = 0;
		while(true) {
			//num = num + 1;
			num++;
			System.out.println(num); // 무한 루트에 빠진 
		}	
		//System.out.println("호랑이");	
		
	}	
}

//ex 28-2) 이렇게 사용하는 경우는 없다. 

public class Hello 
{
	public static void main(String[] args) 
	{
		int i = 0;
		while(i < 10) {
			i++;
			System.out.println(i);  
		}	
		System.out.println("호랑이");	
		
	}	
}

//ex 28-3) while 문장 탈출 방법

public class Hello 
{
	public static void main(String[] args) 
	{
		int i = 0;
		while(true) {
			i++;
			
			if( i == 7 ) {
				// 자기자신과 가장 가까이에있는
				// 반복문을 탈출한다.
				System.out.println("탈출 직전");
				break;
			}
			System.out.println(i);  
		}	
		System.out.println("호랑이");	
		
	}	
}

//ex 28-4) 우박수 출력 프로그램 while문 활용

public class Hello 
{
	public static void main(String[] args) 
	{
		int x = 156458;
		int count = 0;
		while(true) {
			count++;
			System.out.println(x);
			if( x % 2 == 0 ) {
				// 홀수
				x = x / 2;
			}else {
				// 짝수
				x = x * 3 + 1;
			}
			
			
			if( x == 1) {
				System.out.println(x);
				System.out.println("탈출 직전");
				break;
			}
			
		}
			System.out.println(count);
			System.out.println("반복문 탈출됨");
	}
}
  
		
```

```java
//ex29) Random 사용 (외부에있는 라이브러리를 끌고온다)

public class Hello 
{
	public static void main(String[] args) 
	{
		// import java.util.Random;
		// 호랑이 tiger = new 호랑이();
		Random rnd = new Random();
		int num = rnd.nextInt();
		System.out.println(num);
		System.out.println(rnd.nextInt());
		System.out.println("-----------------");
		for (int i = 0; i < 4; i++) {
			System.out.println(rnd.nextInt());
		}
		System.out.println("----------------");
		for (int i = 0; i < 4; i++) {
			// 0 ~ 9 
			System.out.println(rnd.nextInt(100));
		}
		
	}	
}
```

```java
//ex30) 

public class Hello 
{
	public static void main(String[] args) 
	{
		//
		Random rnd = new Random();
		for (int i = 0; i < 10; i++) {
			int ct = 0;
			while(true) {
				int num =  rnd.nextInt(10);
				ct++;
				//System.out.println(num);
				if (num == 7){
					System.out.println("탈출 직전");
					break;
			   }			
			}
			System.out.println(ct);
		}
		

			int sum = 0;   // 위에 값을 누적하는 코드
  // sum = sum + i;
		for (int i = 0; i < 50; i++) {
			int ct = 0;
			while(true) {
				int num = rnd.nextInt(100);
				ct++;
				//System.out.println(num);
				if (num == 30 ) {
					break;
				}
			}				
			System.out.println("탈출됨 : " + ct);
			sum = sum + ct; 

		}

		System.out.println("지금까지의 종합은 :" + sum);
		System.out.println("지금까지의 평균은 :" + sum/50);
	}

}
```

```java
//ex31) 

public class Hello 
{
	public static void main(String[] args) 
	{
		for (int i = 0; i < 10; i++) {
			System.out.println("호랑이 : " + i);
			if( i == 4 ) {
				break;
			}
		} 
		
		System.out.println("탈출됨------------------------");
		
		for (int i = 0; i < 10; i++) {
			if( i == 4 ) {
				continue;
			}
			
			if ( i == 7 ) {
				break;
			}
			System.out.println("호랑이 : " + i);
		} 
		System.out.println("----------------------------");
		
		Random rnd = new Random();
		while(true) {
			int num = rnd.nextInt(100);
			
			// 3의 배수를 잡으면 이 프로그램은 무한루프에 빠진다.
			if ( num % 2 == 0 || num % 5 == 0 ) {
				System.out.println("짝수 혹은 5의 배수");
				continue; // 파일문으로 올라간다.
			}
			System.out.println(num);
			if(num == 99) {
				break; // 탈출 시킨다.
			}
		}
	}	
}
```

```java
//ex32) 배열

public class Hello 
{
	public static void main(String[] args) 
	{
		// array
		// 4byte 짜리 메모리 10개를 달라.
		//int[] arr = new int [10];		
		// 4 * 10 = 40byte
		// 배열을 초기값으로 받았을때 메모리가 0으로 클러어 된다.
		int[] arr = new int[10];
		int[] tiger = new int[10];							   
		//arr[10] >> 이런 변수명은 없다.

		//ex1)
		arr[0] = 3;
		System.out.println(arr[0]);
		
		//ex2)
		System.out.println(arr[1]); // 0이 나온 이유 초기값 받으면 0으로 클리어
       
		//ex3)
		arr[6] = arr[0] * 10;
		System.out.println(arr[6]);
		
		//ex4)
		arr[3] = 999;
		arr[7] = arr[arr[0]]; // 괄호 중첩은 안에있는거 먼저
		//arr[7] = arr[arr[3]] 
		System.out.println(arr[7]);
		
		//ex5)
		arr[9] = 777;
		arr[8] = arr[arr[7]-990];
	    //arr [8] = arr[arr[7]; // 프로그램 설립 안됨.
		//arr[8] = arr[999-990]; //사용 가능 숫자 0~9 이렇게 하면 설립 가능.
		
		System.out.println(arr[8]);
		
		//ex6) 변수도 사용할수 있다.
		System.out.println("------------------------");
		for (int i = 0; i < 10; i++) {
			System.out.print(arr[i]+ " ");
		
		// 12345678
		//ex7) 변수도 사용할수 있다.
		System.out.println("------------------------");
		System.out.println("배열의 크기 : " + arr.length);
		//for (int i = 0; i < arr.length; i++) {
			System.out.println(arr[1]+" ");
		}		
		System.out.println();
		
		//ex8) 아주 중요합니다. 
		// arr[10] = 666; // 프로그램 중단됨
		// java.lang. Array Index Out Of Bounds Exception ( 자바 경계영역을 벗어났다 )
		// 해석보단 구글링 우선으로 빠르게 해결.
		System.out.println("호랑이");
	}
		
}

```

```java
//ex33)

public class Hello 
{
	public static void main(String[] args) 
	{
		// 1. 정석 
		int[]ar = new int [10];
		
		// 2. 데이터 초기화 
		int[]br = new int [] {10, 20, 30, 40, 50};
		System.out.println(br.length);
		
		// 3. 약식 
		int[]cr = {1, 2, 3, 4, 5, 6, 7, 8, 9};
		for (int i = 0; i < cr.length; i++) {
			System.out.print(cr[i] + " ");
		}System.out.println();
		
		//4. etc : 전형적인 예제
		int num = 10;
		int[]dr = new int[num];
		System.out.println(dr.length);		
				
		
		
	}	
}
```

```java
// 자바가 익숙해지면 그때 2차원 배열 이상을 해보세요.
//ex34) 2, 3, 4, 5, 3, 7, 8, 7
// 		 결과 : 9  11,11, 8,

public class Hello 
{
	public static void main(String[] args) 
	{
		//ex 1)
		int[] ar = {2, 3, 4, 5, 3, 7, 8, 7, 6, 2};
//		System.out.println(ar[0] + ar[7]);
//		System.out.println(ar[1] + ar[6]);
//		System.out.println(ar[2] + ar[5]);
//		System.out.println(ar[3] + ar[4]);
		
		for (int i = 0; i < ar.length; i++) {
	        //System.out.println(i + " "+ (7-1));
			System.out.print(ar[i] + ar[ar.length-1 -i] + " ");
		}System.out.println();
		
		
		//ex 2)
		Random rnd = new Random();
		int num = 20 ;
		int[]br = new int[num];
		for (int i = 0; i < br.length; i++) {
			br[i] = rnd.nextInt(10); // 로직
		}
		
		for (int i = 0; i < br.length; i++) {
			System.out.print(br[i] + " ");
		}System.out.println(); // 디스플레이
		
		// 앞과 뒤의 데이터를 순차적으로 더 한다.
		for (int i = 0; i < br.length; i++) {
			System.out.print(br[i] + br[br.length-1 -i] + " ");
		}System.out.println();
		
		//ex 3)
		// 데이터를 설정하는 간단한 예제
		int[]cr = new int[10];
		for (int i = 0; i < cr.length; i++) {
			cr[1] = i * 10 + i;
			//cr[1] = i *  i + i * + i;
		}
	}
}
```

```java
//ex35) 
// 클래스 이름의 첫글자만 대문자로 하는것이 관례이다.
class Airplane{
	// 0. 생성자
	
	// 1. 속성(변수 >> 필드(field)) 
	int num; // (3). 변수가 있으니까 제공하겠다.
	char a1;
	boolean a2;
	long color;
	float pi;
	
	// 2. 동작(함수 >> 메쏘드(method)) 
}

public class Hello 
{
	public static void main(String[] args) 
	{
		//호랑이 tiger = new 호랑이();
		//객체가 생성되었다. >> 날수있다. 먹을수있다. 사용할수있다.
		Airplane air = new Airplane(); // (1). 클래스 호출 하는데 걔이름을 air로 하겠다.
		System.out.println(air.hashCode());
		
		Airplane air2 = new Airplane();
		System.out.println(air2.hashCode());
		
		air.num = 100; // (2). 내가 클래스에 있는 변수를 쓰겠다.
		System.out.println(air.num);
		System.out.println(air2.num); 
		
		air.color = 200;
		air2.color = 300;
		
		System.out.println(air.color);
		System.out.println(air2.color);
		
	}	
}

```

```java
//ex36) 
class Tiger{
	int fuel = 100;
}

public class Hello {
	public static void main(String[] args) {
		//Tiger  t = new Tiger();
		//Tiger t = new //Tiger();
		Tiger t1 = new Tiger();
		System.out.println(t1.hashCode());
		
		Tiger t2 = new Tiger();
		System.out.println(t1.fuel);
		System.out.println(t2.fuel);
		t1.fuel = t1.fuel - 20;
		t2.fuel = t2.fuel - 30;
		
		System.out.println(t1.fuel);
		System.out.println(t2.fuel);
 	}	
}
```

```java
//ex 37)
class Tiger{
	// 생성자
	// 필드
	// 메소드 (method) : 동작
	
	// 자주 사용되는 코드를
	// 클래스에 저장해서
	// 필요할때 마다 꺼내어서 사용하는것.
	void method01() {  // 객체를 생성하기위해서 메소드를 입력한후 진행된다.
		System.out.println(33);
		System.out.println("저는 매쏘드");
		System.out.println(44);
	}
	void meth() {
		int sum = 0;
		for (int i = 1; i <= 10 ; i++) {
			 sum = sum + i;
			
		}
		System.out.println(sum);
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger t1 = new Tiger();
		System.out.println(1);
		t1.method01(); // 메쏘드 콜이 일어난다.
		
		System.out.println(2);
		
		t1.method01(); // 메쏘드 콜이 일어난다.
		
		System.out.println(3);
		
		t1.method01(); // 매쏘드 콜이 일어난다.
		
		System.out.println("----------------------");
		t1.meth();
		System.out.println(4);
		
		
		System.out.println(t1.hashCode()); // 명령어  > 잘 만들어진 메쏘드 
		
	}	
	
}

```

```java
//ex38)
class Tiger{
	// 유형1)
	// 리턴 :  X  전달값 : X
	void m1() {
		System.out.println("멍");
	}
	//유형2)
	// 리턴 : X   전달값 : O
	// int num = 5; 대입연산자가 작동한다.
	void m2(int num) {
		for (int i = 0; i < num; i++) {
			System.out.print("멍");
		}System.out.println();
	}
	
	void m3(int num) {
		int sum = 0;
		for (int i = 1; i <= num ; i++) {
			 sum = sum + i;
			
		}
		System.out.println(sum);
	}
	void m4(int dan) {
		for (int i = 0; i < 10; i++) {
			System.out.println(dan + "*" + " " + i*dan);
		}
		System.out.println("--------------------");
	}
}

public class Hello {
	public static void main(String[] args) {
	  Tiger t = new Tiger();
	  t.m1();
	  t.m2(15);
	  t.m3(100);
	  t.m3(1000);
	  for (int i = 0; i < 5; i++) {
		  t.m4(i*3+1);
	   	    
		}
	}	
}

```

```java
//ex39) 
class Tiger{
	// 유형2)
	// 리턴 : X   전달값 : O
	//void m1(int a,b) {  이렇게는 안된다
	//void m1(int a, int b) { // 이렇게 수식어를 작성
	void m1(int w, int h, char ch) {	// width , height
		for (int i = 0; i < h; i++) {
			for (int j = 0; j < w; j++) {
				System.out.print( ch + " ");
				
			}
			System.out.println();
		}
	}
	void m2(int width, int height, char ch1, char ch2) {
		for (int i = 0; i < height; i++) {
			for (int j = 0; j < width; j++) {
				if((i + j) % 2 == 0 ) {
					System.out.print(ch1 + " " );
				}else {
					System.out.print(ch2 + " " );
				}
			}
			System.out.println();
	   }
	}	
}

public class Hello {
	public static void main(String[] args) {
	   Tiger t = new Tiger();
	   char ch = 'o';  // 대입연산 발생
	   t.m1(10, 8, 'ㅎ');
	   t.m2(7, 10, 'U', '.');
	}	
}
```

```java
//ex40) return을 사용하는 경우는
// 메쏘드가 수행한 결과값을 호출한측으로 돌려 주고 싶을때 < 리턴의 뜻 >
class Tiger{
	// 유형3)
	// 리턴 : O   전달값 : X
	// void =  return이 없다. , int = return이 있다.
	// int m1() {  =인트가 리턴 된다. 
	// return 예약어가 반드시 있어야 한다.
	int m1() {
		System.out.println("멍");
		return 100;
	}
	void m2() {
		System.out.println("야옹");
	}
}

public class Hello {
	public static void main(String[] args) {
	   Tiger t = new Tiger();
	   // 1. 외면
	   t.m1();
	  
	   // 2. 받아서 사용하는 경우
	   int num = t.m1();
	   System.out.println(num);
	   
	   // 3. 받는 절차를 생략하고 출력해버린다.
	   System.out.println(t.m1());
	   
	   // 주의 : 사용 할 수 없음.
	   //System.out.println(t.m2());
	}	
}

```

```java
//ex41) 리턴값에 대한 심화 가능 불가능에 대한
class Tiger{
	// 유형4)
	// 리턴 : O   전달값 : X
	int m1(int a, int b) {
		int sum = a + b;
		return sum;
		// =return a + b; 같은 의미 ( 리턴받을 값을 재활용 하기 힘들다.)
	}	
		void m2(int a, int b) {
			int sum = a + b;
		  System.out.println(sum);
	}
}

public class Hello {
	public static void main(String[] args) {
	   Tiger t = new Tiger();
	   		
	   int ss = t.m1(10, 20);
	   System.out.println(ss);
	   
	   System.out.println(t.m1(30, 40));
	   
	   t.m2(3, 4);
	   
	   System.out.println(t.m1(1, 2) * t.m1(3, 4));
	}
}
```

```java
//ex42) 메쏘드 원형 ( 함수 원형 ) proto type
class Tiger{
	// 리턴 : X   전달값 : X
	void m1( ) { }
		
	// 리턴 : X   전달값 : O
    void m2(int a, int b ) { }
   
 // 리턴 : O   전달값 : X
    int m3() { return 0; }
   
 // 리턴 : O   전달값 : O
    int m4(int a, int b) { return 0; }
		
}

public class Hello {
	public static void main(String[] args) {
	   Tiger t = new Tiger();
	}	
}
```

```java
//ex43) 
class Tiger{
	// 필드, 메쏘드,  생성자 : 멤버(가족)
	// 생성자는 <필드 초기화를 목적>으로 한다. ( 그게 끝이다. )
	// int x=10, y; 이것도 초기화 가능 
	// 생성자(method) 의 정확한 용어는 생성자 메쏘드이다.
	// 생성자의 이름은 반드시 클래스 이름과 동일해야 한다.
	// 생성자 함수는 retrun값을 가질수가 없다.
	//    그래서 void 예약어 조차 적지 않는다.
	// 생성자 함수는 자동 호출 된다.
	//         언제) 객체가 생성될때..
	//         생성이 뭔데 ? ) new를 사용할때
	// 자동생성자 호출을 제외하고 <임의로 생성자함수를 호출 할수 없다..
	// retrun값은 가질수 없지만 인수 전달은 할수 있다.
	
	int x, y; // 필드
	
	Tiger(int a, int b) { 
		System.out.println("생성자 콜");
		x = a;
		y = b;
	}
	void showData() {
		System.out.println(x + " " + y);
	}
}

public class Hello {
	public static void main(String[] args) {
	    System.out.println(1);
		Tiger t = new Tiger(10, 20); // 객체가 생성된것, 호출한것
		System.out.println(2);
		Tiger t2 = new Tiger(30, 40); // 새로운 객체 생성
		t.showData();
		t2.showData();
	}	
}
```

```java
//ex44) 생성자의 기본적이 글꼴
class Tiger{
	// 무의미한 코드
	//int x=777, y=888;   // 실행1)
	int x, y;			        // 실행1)
	Tiger(int a, int b){  // 실행2)
		x = a;
		y = b;
	}
	void showData() {
		System.out.println(x + " " + y);
	}
}

public class Hello {
	public static void main(String[] args) {
	   Tiger t1 = new Tiger(1, 2);
	   Tiger t2 = new Tiger(10, 20);
	   
	   System.out.println(t1.x + " " + t1.y);
	   System.out.println(t2.x + " " + t2.y);
	   
	   Tiger t3 = new Tiger(100, 200);
	   System.out.println(t3.x + " " + t3.y);
	   System.out.println("----------------------");
	   t1.showData();
	   t2.showData();
	   t3.showData();
	}	
}
```

```java
//ex45) 오버로딩 
class Tiger{
	// 전달되는 연수의 개수가 다르면 함수이름을 동일하게 사용할수 있다.
	// 전달되는 연수의 개수가 같더라도 연수의 타입이 다르면
	// 같은 이름 사용 할수 있다.
	
	// 메쏘드 오버로딩 
	// 같은 이름으로 메쏘드 이름을 정의 하기 위하여
	// 1. 전달되는 연수의 개수가 다르든지
	// 2. 개수가 같더라도 받는 타입이 다르면 사용할수 있다.
	void showMeTheMoney() {
		System.out.println(1000);
	
	}		
     void showMeTheMoney(int num) {
    	  System.out.println(2000);
     }
     void showMeTheMoney(int num,int count) {
    	  System.out.println(3000);  // 오버로딩 됨
     }
     void showMeTheMoney(float num) {
    	  System.out.println(4000);  // 오버로딩 됨
     }
     
}

public class Hello {
	public static void main(String[] args) {
	   Tiger t = new Tiger();
	   t.showMeTheMoney();
	   t.showMeTheMoney(1); // 맵핑이 된다. (연결이 된다)
	   t.showMeTheMoney(1, 2);
	   
	   
	}	
}
```

```java
//ex46) 생성자 오버로딩 ( overloading ) 
class Tiger{
	Tiger(){
		System.out.println(1);
	}
	Tiger(int a){
		System.out.println(2);
	}
	Tiger(int a, int b){
		System.out.println(3);
	}
	Tiger(float a){
		System.out.println(4);
	}
	
	
}

public class Hello {
	public static void main(String[] args) {
	   Tiger t1 = new Tiger();
	   Tiger t2 = new Tiger(10);
	   Tiger t3 = new Tiger(10, 20);
	   Tiger t4 = new Tiger(3.14f);
	}	
}
```

```java
//ex47) 상호 호출은 X, 재귀호출은 사용가능 하지만 고급 프로그램에서 사용된다
class Tiger{
	// 1. 필드가 먼저 나타난다.
	int x, y;
	
	// 2. 다음 생성자 메쏘드가 작성된다.
	Tiger(int a, int b){
		x = a * 10;
		y = b * 20;
		
	}

	// 3. 메쏘드 순서로 작성한다.
	void showData() {
		System.out.println(x + " " + y);
	}
	void m1() {
		System.out.println("m1 call");
	}
	void m2() {
		System.out.println("m2 call");
		m1();
		System.out.println("--------------------");
		
	}
	
	// 상호 호출은 사용할수 없다. (수식값이 발생하지 않고 오류가 생겼음.)
	//void m3() {
	//	System.out.println("m3 call");
	//	m4();
	//	}
  //  void m4() {
	//	System.out.println("m4 call");
	//	m3();
	}
    
    // 재귀 호출 : 적당하게 고급 프로그램에서 사용된다. (잘 사용하면 좋다.) 본인이 본인을 호출하는 함수
    void m5() {
		System.out.println("m5 call");
		m5();
	}
	   int m6() {
		System.out.println("호랑이3");
		return 10;
	}
	int m7() {
		System.out.println("호랑이2");
		return m6() * 3; // 10 * 3
	}
	int m8() {
		System.out.println("호랑이1");
		return m7() * 100; // 10 * 3 * 100
		}

	}

public class Hello {
	public static void main(String[] args) {
	   Tiger t = new Tiger(5, 10);
	   t.showData();
	   t.m2();
		//System.out.println(t.m6());
		//System.out.println(t.m7());
			System.out.println(t.m8());
		//t.m3();
		 t.m5();
	}	
}
```

```java
//ex48) 클래스를 만들어본다.
class Airplane{
	int fuel;
	Airplane(){
		fuel = 100;
		
	}
	Airplane(int fl){
		fuel = fl;
	}
	void showFuel() {
		 System.out.println("남은 연료량은 : " + fuel);
	}
	void fly() {
		 System.out.println("날아갑니다. 훨훨.");
		 fuel -= 15; // (fuel = fuel - 15;) 동일함
	}
	void fly(int km) {
		for (int i = 0; i < km; i++) {
			if( fuel < 15 ) {
				System.out.println("연료가 부족합니다.");
				break;
			}
			System.out.println("날아갑니다. 훨훨");
			fuel -=15;
		}
	}
	void inject(int ml) {
		fuel += ml;
		showFuel();
		//System.out.println(fuel); 둘다 가능하다.
	}
}
	

public class Hello {
	public static void main(String[] args) {
		Airplane air1 = new Airplane();
		Airplane air2 = new Airplane(200);
		air1.showFuel();
		air2.showFuel();
		
		
		int num = 10;
		num = num + 1;
		num++;
		System.out.println(num);
		num = num + 3;     // 1. 프로그램 : 컴파일 속도가 느리다. (직관적으로 한다)
		num += 3;		   // 2. 프로그램 : 컴파일 속도가 빠르다. (직관적으로 해석을 하려해서 가속성 떨어짐) 겉멋
		// 복합대입연산자는
		// 산술, 비교, 관계연산 모두 성립된다. 
		System.out.println(num);
		System.out.println("-----------------------------");
		air1.fly();
		air1.showFuel();
		
		for (int i = 0; i < 3; i++) {
			air2.fly();
		}
		air2.showFuel();
		air2.fly(5);
		air2.showFuel();
		
		air2.fly(10);   
		air2.showFuel();
		air2.inject(400);
	}	
}
```

```java
//ex49-1)
class A{

}

class B{
	void f1() {
		System.out.println("나는 f1");
	}
	void f2() {
		System.out.println("호랑이");
	}
}

class C{
	void f1() {
		System.out.println("나는 f1");
	}
	void f2() {
		System.out.println("코끼리");
	}
}

public class Hello {
	public static void main(String[] args) {
		B t1 = new B();
		C t2 = new C();
		t1.f1();
		t1.f2();
		t2.f1();
		t2.f2();
	
	}
	
}

//ex49-2) // 상속관계 기본 형식
class A{
		void f1() {
			System.out.println("나는 f1");
		}

}
// 부모가 A, 자식B
class B extends A{
	void f2() {
		System.out.println("호랑이");
	}
}
//부모가 A, 자식 C
class C extends A{
	void f2() {
		System.out.println("코끼리");
	}
}

public class Hello {
	public static void main(String[] args) {
		B t1 = new B();
		C t2 = new C();
		t1.f1(); 
		t1.f2();
		t2.f1();
		t2.f2();
	
	}
	
}
```

```java
//ex50) 상속구조의 전형적이 모습.(상속의 상속관계도 가능하다.)

class Aaa{
	void f1() {
		System.out.println("Aaa f1");
	}
	void f3() {
		System.out.println("Aaa f3"); // 직접적으로 사용 불가.
	}

}

class Bbb extends Aaa{
	void f2() {
		System.out.println("Bbb f2");
	}
	void f3() {
		System.out.println("Bbb f3");
	}
	void f4() {
		f3();
		super.f3(); // 부모의 키워드를 사용하게 만드는 super 
		//super.f1(); 굳이 super 붙일 필요없이 f1으로 작동 시킬수 있다.
	}

}

public class Hello {
	public static void main(String[] args) {
		Bbb t = new Bbb();
		t.f1();
		t.f2();
		t.f3();
		System.out.println();
		t.f4();
	}
	
}
```

```java
//ex51) extends 

class Aaa{
	void f1() {
		System.out.println("조"); // 조부
	}
}
class Bbb extends Aaa{
	void f2() {
		System.out.println("부"); // 부모
	}
}
class Ccc extends Bbb{
	void f3() {
		System.out.println("자"); // 자신
	}
}

public class Hello {
	public static void main(String[] args) {
		Ccc t = new Ccc();
		t.f1();
		t.f2();
		t.f3();
	}
	
}
```

```java
//ex52) 자식은 부모하다 ( is a 관계 ) 
// 호랑이는 동물이다.
class Animal{

}
class Tiger extends Animal{
	
}
// 가문법적으로 성립이 되더라도 말도 안되는 상속구조
class rabbit extends Tiger{
	
}

class 도형{
	
}
class 삼격형 extends 도형{
	
}
class 사각형 extends 도형{
	
}

// has a 관계
class 무기{}
class 경찰 extends 무기{}
class 범인 extends 무기{}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger();
	
	}
	
}
```

```java
//ex53) String의 정의

class Tiger{
	void f1() {
		
	}
	void f2() {
		
	}
}

public class Hello {
	public static void main(String[] args) {
		// 첫글자가 대문자를 씀으로써 class문법 이다. , 8개가 원시 타입이다.
		// int apple = "호랑이"; // 사용 해본적 없다.
		System.out.println("호랑이");
		// 문자열만 전문적으로 관리해주는 class 이다.
		Tiger t1 = new Tiger();
		t1.f1();
		System.out.println("-------------------");
		String s1 = new String("코끼리"); // 초기값을 정해두고 사용하는 방법.
		System.out.println(s1);
		
		String s2 = new String();
		s2 = "독수리";
		System.out.println(s2);
		
		String s3 = "앵무새꽃이피었습니다";  // String 에서 사용하기 좋은 length
		System.out.println(s3);
		System.out.println(s3.length());
		
		// 이런 class도 있다.
		Thread th = new Thread();
		
	}

		
}
```

```java
//ex54)

class Tiger{
	void f1() {
		
	}
	// void f2(숫자, 문자열 class)
	void f2(int num, String s) {
		System.out.println(num);
		
		for (int i = 0; i < num; i++) {
			System.out.println(s);
		}
	}

}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger();
		//t.f2(100, 200);
		//t.f2(100, "한");
		//t.f2(100, 3.14f);
		t.f2(4, "문자열전달");
	}
	
}
```

```java
//ex55) 객체값을 생성해서 리턴값을 제공했는데 결국 리턴값을 무시하고 진행됐다.

class Tiger{
	void rich() {
		System.out.println("Tiger의 rich호출됨");
	}

}
class Lion{
	// (class , class)
	void f1(String s, Tiger t) {
		System.out.println(s);
		System.out.println(s.length());
		t.rich();
	}
	
	Tiger f2() {
		Tiger t = new Tiger();
		return t; // 리턴받은 값을 무시했다.
	}
}

public class Hello { 
	public static void main(String[] args) {
		Lion lion = new Lion();
		lion.f1(new String("호랑이"), new Tiger());
		//String s = new String("호랑이");
		//Tiger t = new Tiger();
		lion.f2();
		Tiger t = lion.f2();
		t.rich();
	}
	
}
```

```java
//ex56-1) static 의 개념

class Airplane{
	 //static int 관재탑; 메모리 존재유무에 관계있다.
	 static int count;
	 int num;
	 void fly() {
		
	}

}

public class Hello {
	public static void main(String[] args) {
		Airplane t1 = new Airplane();
		Airplane t2 = new Airplane();
		Airplane t3 = new Airplane();
	
	}
	
}

//ex56-2)

class Airplane{
	 //static int 관재탑; 메모리 존재유무에 관계있다.
	 static int count = 100;
	 int num;
	 void fly() {
		
	}

}

public class Hello {
	public static void main(String[] args) {
		// class이름.static변수명
		System.out.println(Airplane.count);
		Airplane.count = Airplane.count + 100;
		System.out.println(Airplane.count);
		//System.out.println(Airplane.num); 성립안된다.
		
		Airplane a1 = new Airplane();
		System.out.println(a1.count);
		a1.count = 1000;
		System.out.println(Airplane.count);
			
	}
	
}

//ex56-3)

class Tiger{
	static int count = 10;
	int num = 20;
	static void f1() {
		System.out.println("call");
	}

	void f2() {
		 count++;
	}
	
	static void f3() {
		count++;
		// num++; static 함수 안에서는 static 멤버만 사용할수 있다.
		// static 멤버 ( 필드 ,  메소드 )
		// 저 함수는 error
	}
}

public class Hello {
	int apple;
	
	void f1() {
		apple = 20;
	}
	
	public static void main(String[] args) { // 운영체제를 호출하기위해서 static를 입력해야 호출가능.
		//Tiger t = new Tiger();
		Tiger.f1();
		Tiger t = new Tiger();
		t.f1();
		//apple++; 이건 사용불가.
		//f1(); 이것도 불가능.
	
	}
	
}

//ex56-4)

class Tiger{
	void f1() {
		Tiger t = new Tiger();
	}
}

public class Hello {
	int num;
	Hello(){
		
	}
	void f1() {
		System.out.println(100);
	}
	public static void main(String[] args) {
		Hello h = new Hello();
		h.f1();
		//f1(); 이건 불가능.
	
	}
	
}

```

```java
//ex57)

class Tiger{
	static int abs(int a) {
		if( a < 0 ) {
			a= -a;
		}
        return a;
    }
}
public class Hello {
	public static void main(String[] args) {
		Math.abs(-20); 
		// Math.abs(-20); static 함수
		// Math m = new Math();
		// m.abs(0;)
		System.out.println(Math.abs(-20));
		System.out.println(Tiger.abs(-20));
		
		//Thread.sleep(0);
	}
	
}
```

```java
//ex58-1) 
// final 을 사용할수 있는곳은 3곳.

final class Tiger{
	// 1. field명 앞에 붙이는 경우
	// 값을 대입받는곳이 여기가 마지막이다.
	// 불변의 값을 초기화하고 사용할때
	final int num = 10;
	
}
// 부모가 final이기 때문에 상속을 할수 없다.
//class Lion extends Tiger{
//	void f1() {
//		
//	}
// }

class A{}
final class B extends A{}
// class C extends B{}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger();
		System.out.println(t.num);
		// 값을 대입할수 있으면 변수.
		// 값을 대입할수 없는것은 상수.
		System.out.println(Math.PI); 
		// t.num = 20;  사용할수 없다.
	
		String s = "호랑이";
	}
	
}

//ex58-2)

class Aaa{
	// method Overloading
	void f1() {}
	void f1(int a) {}
	
	void f2(int a, String s) {}
	// 3. final 때문에 오버라이딩이 금지 된다
	final void f3() {}
}
class Bbb extends Aaa{
	// overriding
	void f2(int a, String s) {
		System.out.println(a+s);
	}
	// 3. 부모의 final 때문에 오버라이딩 할수 없다.
	// void f3() {}
}

public class Hello {
	public static void main(String[] args) {
		Bbb t = new Bbb();
		t.f2(10, "토끼");
	}
	
}
```

```java
//ex59-1)
// 이 class는 추상 함수를 포함하고 있다. 추상함수는 객체를 생성할수 없다.
// 미완성 class는 자식이 상속을 받아서 완성하세요.
abstract class Tiger{
	void f1() {
		System.out.println(10);
	}
	// 이 함수가 추상함수 ( 미완성 함수 )
	abstract void f2(); // 미완성 코드 (추상 함수)
}

class Lion extends Tiger{
	void f2() { // 오버라이딩
		System.out.println(20);
	}
}
public class Hello {
	public static void main(String[] args) {
		// code가 미완성이기 때문에 객체를 생성할수 없다.
		// Tiger t = new Tiger();
		Lion t = new Lion();
		t.f2();
		t.f1();
	}
	
	
}

//ex59-2) 추상함수 

abstract class 대장장이{
	void 칼만들기() {
		System.out.println("멋진 칼만듦");
	}
	abstract void 방패(); 
		//System.out.println("허접 방패");
	
}
class 방패쟁이 extends 대장장이{
	void 방패 () {
		System.out.println("멋진 방패");
	}
}

public class Hello {
	public static void main(String[] args) {
//		대장장이 t = new 대장장이();
//		t.칼만들기();
		방패쟁이 t = new 방패쟁이();
		t.칼만들기();
		t.방패();
	
	}
	
}
```

```java
//ex60-1)

abstract class Aaa{    		// 완성된 코드가 없고, 구현해야한다.
	abstract void f1();		// 인터페이스 ( 실행되는 파일이 없다. 그래서 구현해줘야 한다. )
	abstract void f2();	
	abstract void f3();
}
class Bbb extends Aaa{ 		// 구현완료
	void f1() {}
	void f2() {}
	void f3() {}
}
public class Hello {
	public static void main(String[] args) {
		 
	}
	
}

//ex60-2) interface

interface Aaa{    		
	 void f1(); // 	abstract void f1(); (같은 의미)	
	 void f2();	
	 void f3();
}
class Bbb implements Aaa{     // implements		
	public void f1() {
		System.out.println(1);
	}
	public void f2() {
		System.out.println(2);
	}
	public void f3() {
		System.out.println(3);
	}
}
public class Hello {
	public static void main(String[] args) {
		 Bbb t = new Bbb();
			t.f1();
		 	t.f2();
		 	t.f3();
	}
	
}
```

```java
//ex 61)

interface 한국은행{
	void 입금();
	void 출금();
	// 등등..

}

class 하나은행 implements 한국은행{
	public void 입금() {
		System.out.println("입금됨");
	}
	public void 출금() {
		System.out.println("출금됨");
	}
	void 입출금() {
	 System.out.println("이자는 5%이다.");	
			
		
	}
}
class 우리은행 implements 한국은행{
	public void 입금() {
		System.out.println("입금됨");
	}
	public void 출금() {
		System.out.println("출금됨");
	}
	void 입출금() {
	 System.out.println("이자는 5%이다.");	
			
		
	}
}
public class Hello {
	public static void main(String[] args) {
		하나은행 t = new 하나은행();
		t.입출금();
	}
	
}
```

```java
//ex62)

class A{
	void f1() {
		System.out.println();	
	}

}
class B{
	void f2() {
		System.out.println();
	}
}
class C{
	void f3() {
		System.out.println();
	}
}
class D{
	void f4() {
		System.out.println();
	}
}
 class E extends A implements C, D {
	void f5() {
		
	}
	public void f3() {
		
	}
	public void f4() {
		
	}
}

public class Hello {
	public static void main(String[] args) {
		E t = new E();
			t.f1();
			t.f5();
			t.f3();
			t.f4();
	}
	
}
```

```java
//ex63)

abstract class A{
	 abstract void f1();
	
}
// interface가 선호된다.
interface B{
	void f1();
}

class C extends A{
	@Override // 간접적으로 설명한다, 에러 방지용 ( @ = 어노테이션 ) 
	void f1() {
		System.out.println(100);
		
	}
}

class D implements B{
	@Override // 어노테이션
	public void f1() {
			System.out.println(200);	
	}
}
public class Hello {
	public static void main(String[] args) {
		C t1 = new C();
		t1.f1();
		D t2 = new D();
		t2.f1();
	
	}
	
}
```

```java
//ex64-1)

class Tiger{
	// 생성자
	Tiger(){
		System.out.println(1);
	}
	Tiger(int a){ 
		System.out.println(2);
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger t1 = new Tiger();
		Tiger t2 = new Tiger(100);
	
	}
	
}

//ex64-2)

class Tiger{
	// 자동 완성 코드 1
	// Tiger(){}
	
	// 자동 완성 코드 1
	// Tiger this; 
	int num = 100;
	Tiger air01; // = new Tiger();
	void f1() {
		air01 = new Tiger();
		System.out.println(air01.num);
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger air2;  // = new Tiger();
		air2 = new Tiger();
		air2.f1();
		
	
	}
	
}

//ex64-3)

class Tiger{
	// 생략 1
	// Tiger(){
	//  this =  t1;
	// }
	// 생략 2
	// Tiger this;
	// 생략 3
	
}

public class Hello {
	public static void main(String[] args) {
		Tiger t1 = new Tiger();
	
		
		Tiger t2 = t1; // 객체는 1개인데 동일한 객체로 만든다.
		
		System.out.println(t1.hashCode());
		System.out.println(t2.hashCode());
		
	}
	
}

//ex64-4) this 임의로 들어가 있다. t = this 

class Tiger{
	Tiger(){
		System.out.println(this.hashCode());
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger();
		System.out.println(t.hashCode());
	}
	
}

//ex64-5)

class Tiger{
	// Tiger this;
	// Tiger(){
		// 공유 코드를 만든다.
		// this = apple
	// }
	
	int num = 100;
	void f1() {
		System.out.println("콜됨");
		// System.out.println(num); // 정산 코드가 아니다.
		System.out.println(this.num);
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger apple = new Tiger();
		System.out.println(apple.num);
		apple.f1();
	}
	
}
```

```java
//ex65-1) this 를 사용하는 이유 1
 
class Tiger{
	int apple, banana;
		
	Tiger(int apple, int banana) {
		
		this.apple = apple;
		this.banana = banana;
	}

	int add() {
		return this.apple + this.banana;
		// return apple + banana; (this 생략)
	}
	void f1() {
		System.out.println("원숭이");
	}
	void f2() {
		this.f1();
		// f1(); (this가 생략)
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger air = new Tiger(10, 20);
		System.out.println(air.add());
		
		int num = 10;
		num = num;
		
		air.f2();
	}
	
}

//ex65-2) 

class Tiger{
	void f1() {
		
	}
	int f2() {
		return 100;
	}
	String f3() {
		return "호랑이";
	}
	Tiger f4() {
		return new Tiger();
	}
	Tiger f5() {
		return this; 
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger();
		Tiger t2 = t.f5();
		System.out.println(t.hashCode());
		System.out.println(t2.hashCode());
	
	}
	
}

//ex65-3) this 를 사용하는 이유 2 ( 체이닝 ) 

class Tiger{
	void f1() {
		System.out.println(1);
	}
	Tiger f2() {
		System.out.println(2);
		return this;
	}
	Tiger f3() {
		System.out.println("아침 먹음");
		return this;
	}
	Tiger f4() {
		System.out.println("점심 먹음");
		return this;
	}
	Tiger f5() {
		System.out.println("저녁 먹음");
		return this;
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger();
		t.f2().f2().f2().f1();  // 체이닝
	
		t.
		f3().
		f4().
		f4().
		f4().
		f5();
	}
		
}
```

```java
//ex66) this 를 사용하는 이유 3 ( 생성자 안에서 생성자 호출 )

class Tiger{
	int test;
	Tiger(){
		test = 9999;
		System.out.println("콜1");
	}
	Tiger(int num){
		// 인수 전달이 없는 생성자를 호출합니다.
		this(); 
		System.out.println("콜2");
	}
	Tiger(int a, int b){
		this(a+b); 
		System.out.println("콜3");
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger(100, 200);
	
	}
	
}
```

```java
//ex67) this 심화 과정

class Man{
	int money = 1500;
	void merry() {
		Women w = new Women();
		w.merry(this);
		
	}
	int 재산() {
		System.out.println("500원");
		return money;
	}
	String 성격() {
		//return "포악";
		return "온난";
	}
}
class Women{
	void merry(Man mm) {
		int money = mm.재산();
		if( money < 1000) {
			System.out.println("싫어요1.");
		}
		if( mm.성격() == "포악") {
			System.out.println("싫어요2.");
		}else {
			System.out.println("OK...");
		}
		
		
		// Yes or No
	}

}

public class Hello {
	public static void main(String[] args) {
		Man man = new Man();
		man.merry();
	}
	
}
```

```java
//ex68) 문자열 사용법

public class Hello {
	public static void main(String[] args) {
		String s = "무궁화꽃이피었습니다";
		
		// 1.
		System.out.println(s.length()); // 이 사용법 유용하다
		
		// 2.
		// char charAt(int index) 
		char ch = s.charAt(9);
		// char ch = s.charAt(3); //리턴하는 문자의 3번째 문자를 찾아달라.(charAt)
		System.out.println(ch);
		
		// 3. int indexOf(int ch)
		System.out.println(s.indexOf("심피었")); // -1 일 경우는 못찾았다.
		
		int indexNum = s.indexOf("심피었");
		if(indexNum == -1 ) {
			System.out.println("검색 실패");
		}else {
			System.out.println("검색 성공");
		}
		
		// 4. String java.lang.String.replace(CharSequence target, CharSequence replacement)
		// 바쿼치기 ( replace )
		String result = s.replace("꽃이", "나무가");
		System.out.println(result);
		System.out.println(s); // 원본
		
		// 5. String java.lang.String.substring(int beginIndex)
		// 잘라내기 ( substring )
		System.out.println(s.substring(3));
		System.out.println(s.substring(2, 8)); // 함수 오버로딩 적용된다.
	
		// 6. 대문자, 소문자 전체 변경하는 법
		String s2 = "Apple";
		System.out.println(s2.toLowerCase());
		System.out.println(s2.toUpperCase());
		System.out.println(s2);
	}
	
}
```

```java
//ex69) 숫자 >> 문자열 , 문자열 >> 숫자

public class Hello {
	public static void main(String[] args) {
		// 숫자 >> 문자열 변경 ( int >> String )
		
		// 문자열 >> 숫자 ( Strinf >> int )
		
		int num01 = 456;
		System.out.println(num01 + 100);
		
		//숫자 >> 문자열 변경 ( int >> String )
		// "456" 
		String s1 = Integer.toString(num01);
		System.out.println(s1 + 500); //  숫자와 문자열이 합쳐진 결과 나옴
	
		String s2 = "" + num01;
		System.out.println(s2 + 500);
		
		//문자열 >> 숫자 ( Strinf >> int ) Integer.(parseInt)
		String s3 = "6789";
		System.out.println(s3 + 1000);
		
		
		int num02 = Integer.parseInt(s3); // 구문을 분석한다.
		System.out.println(num02 + 1000);
		
		for (int i = 0; i < args.length; i++) {
			
		}
	}
	
}
```

```java
//ex70)

class Tiger{
	//default int data;  // 접근 제한자.
	//public int data;
	private int data;
	

	int getData() {
		return data;
	}
	void setData(int data) {
		this.data = data;
	}
	void f1() {
		data = 200;
		this.data = 200;
	}
	void showData() {
		System.out.println(data);
	}
}

public class Hello {
	public static void main(String[] args) {
		Tiger t = new Tiger();
		//t.data = 999; 이렇게는 사용 안한다.
		t.setData(999);
		t.showData();
		System.out.println(t.getData());
		// 밑에 코드는 실전에서 사용 안된다.
		// data 은닉
		
		
		//t.data = 100;
		//System.out.println(t.data);
	}
	
}
```

```java
//ex71-1)

class Tiger{
	private int data;

	int getData() {
		return data;
	}

	void setData(int data) {
		this.data = data;
	}
	
}
class Cat{
	private float data;

	String getData() {
		return data;
	}

	void setData(float data) {
		this.data = data;
	}
	
}

public class Hello {
	public static void main(String[] args) {
		Tiger t1 = new Tiger();
		t1.setData(100);
		System.out.println(t1.getData());
		
		Lion t2 = new Lion();
		t2.setData("호랑이");
		System.out.println(t2.getData());
		
		Cat t2 = new Cat();
		t2.setData("호랑이");
		System.out.println(t2.getData());
	
	}
	
}

//ex71-2) 제네릭 문법 , CRUD

class Tiger<T>{
	private T data;
	T getData() {
		return data;
	}
	void setData(T data) {
		this.data = data;
	}

}

public class Hello {
	public static void main(String[] args) {
		// 호랑이 t = new 호랑이();
		Tiger<Integer> t = new Tiger<Integer>();
			t.setData(100);
			System.out.println(t.getData());
			
			Tiger<String> t2 = new Tiger<String>();
			t2.setData("호랑이");
			System.out.println(t2.getData());
			
			Tiger<Boolean> t3 = new Tiger<Boolean>();
			t3.setData(true);
			System.out.println(t3.getData());
			
			// LinkedList data를 관리해주는것.  
      // CRUD =>  ( 데이터를 생성 , 데이터를 읽기 , 데이터를 바꾼다 , 데이터를 삭제 )
			// 제네릭 문법을 이용한 컬렉션.(총 8가지 종류) *LinkedList 중요*
			// String s; 
			LinkedList<Integer> mm = new LinkedList<Integer>();
			System.out.println(mm);
			mm.add(100);
			mm.add(200);
			mm.add(300);
			mm.add(400);
			System.out.println(mm);
			mm.remove(2);
			System.out.println(mm);
			
			
	}
	
}
```
