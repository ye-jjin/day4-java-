# day4 - java 문법

### 연산자

1. 연산자,피연산자란?
- 연산자란 변수나 값의 연산을 위해 사용되는 부호를 의미합니다.
- 피연산자란 연산을 수행하기 위해서 있어야 하는 대상을 의미합니다.

<br>
<br>

2. 연산자의 종류

| 종류 | 연산자 | 설명 |
| --- | --- | --- |
| 산술연산자 | + ,- ,* ,/ ,% | 사칙연산과 나머지 연산 |
| 비교연산자 | > ,< ,>= ,<= , == ,!= | 크고 작음 / 같고 다름을 비교 |
| 논리연산자 | && , || , ! , ^ | 그리고 / 또는 으로 조건을 연결 |
| 대입연산자 | = | 우변의 값을 좌변에 저장 |
| 증감연산자 | ++ , — | 피연산자의 값을 증가 혹은 감소 |

---

### 제어문

1. 제어문이란?
- 코드의 실행 흐름은 위에서 아래로 한 문장씩 순차적으로 진행되지만, 조건에 따라 문장을 건너뛰고, 때로는 같은 문장을 반복해서 수행해야 할 때가 있습니다. 이처럼 프로그램의 흐름을 바꾸는 역할을 하는  문장을 제어문이라고 합니다.

<br>
<br>

2. 제어문의 종류

| 종류 | 이름 |
| --- | --- |
| 조건문 | if문, switch문 |
| 반복문 | for문,while문,do-while문 |

<br>
<br>

3. 조건문
- if문
    - if문은 가장 기본적인 조건문이며, `조건식과 괄호 {}`로 이루어져 있습니다.
    - if문에 사용되는 조건식은 일반적으로 비교 연산자와 논리 연산자로 구성됩니다.

```java
if ( 조건식 ) {
         // 조건식이 참( true ) 일 때 수행될 문장
}
==> 만일 if 조건식이 참이면 괄호 {}안의 문장들을 수행
```

<br>
<br>

- if-else문

```java
if ( 조건식 ) {
         // 조건식이 참 ( true ) 일 때 수행될 문장
} else {
         // 조건식이 거짓 ( false ) 일 때 수행될 문장
}
```

<br>
<br>

- if-else if문

```java
if ( 조건식 1 ) {
         // 조건식 1이 참 ( true ) 일 때 수행될 문장
} else if ( 조건식 2 ) {
         // 조건식 1이 거짓 ( false )이고 조건식 2가 참일 때 수행될 문장
} else if ( 조건식 3 ) {
         // 조건식 1, 2가 거짓 ( false )이고 조건식 3이 참 ( true ) 일 때 수행될 문장
} else {
         // 조건식 1, 2, 3 ... 이 모두 거짓 ( false ) 일 때 수행될 문장
}
```

<br>
<br>

- switc문
    - if문은 조건식의 결과가 참/거짓 두 가지 경우만 존재해서 경우의 수가 많아질수록 조건식이 많아지고 복잡해집니다.
    - switch문은 단 하나의 표현식으로 많은 경우의 수를 처리할 수 있습니다.
    - switch문은 `표현식과 case, break` 으로 구성됩니다.
    
    ```java
    switch ( 표현식 ) {
             case 값1 :
                     // 표현식의 결과가 값 1과 같은 경우 수행될 문장
                     break;
             case 값2 :
                     // 표현식의 결과가 값 2와 같은 경우 수행될 문장
                     break;
             default :
                     // 표현식의 결과가 일치하는 case문이 없을 때 수행될 문장
    ```

<br>
<br>
    
4. 반복문
- for문
    - 어떤 작업이 반복적으로 수행되도록 할 때 사용하며, 반복 횟수를 알고 있을 때 사용하는 것이 적합합니다.
    - for문은 `초기식, 조건식, 증감식`으로 구성됩니다.
    
    ```java
    for ( 초기식; 조건식; 증감식 ) {
             // 조건식이 참일 때 반복 수행할 문장
    }
    ```

<br>
<br>
    

- 향상된 for문
    - 배열에 저장된 값이 반복마다 하나씩 순서대로 읽혀서 변수에 저장됩니다.
    - 향상된 for문은 `타입, 변수명, 배열`로 구성됩니다.
    
    ```java
    for ( 타입 변수명 : 배열 또는 컬렉션 ) {
             //반복할 문장
    }
    ```

<br>
<br>    

- while문
    - 조건식이 참인 동안, 반복적으로 문장을 수행합니다.
    - while문은 `조건식과 괄호 {}`로 구성됩니다.
    
    ```java
    while ( 조건식 ) {
             // 반복 수행할 문장
    }
    ```

<br>
<br>  

- do-while문
    - for문이나 while문은 조건식에 따라 한 번도 실행이 안될 수도 있지만, do-while은 최소 한 번은 실행됩니다.
    - {}를 먼저 실행한 후에 조건식에 따라 실행됩니다.
    
    ```java
     do {
             // 조건식의 결과가 참일 때 수행될 문장
             // 단, 한번은 무조건 실행
    } while( 조건식 );
    ```    


---

### 배열

1. 배열이란?
- 배열이란 같은 종류의 데이터들이 순차적으로 하나의 묶음으로 저장되어 있는 자료구조입니다.
- 같은 타입으로만 생성됩니다.

<br>
<br>

2. 배열의 선언과 생성
- 배열 선언
    - 변수의 타입을 선언하고 배열임을 의미하는 대괄호[]를 붙입니다.
    - 배열을 선언한 것은  참조 변수라고 불리는 배열의 주소 값을 가지며 그 자체가 배열은 아닙니다.
- 배열 생성
    - 배열을 선언한 다음 배열을 생성하며 값을 저장할 수 있는 공간을 만듭니다.
    
    | 선언 방법 | 설명 |
    | --- | --- |
    | 타입 배열 이름[]; | 배열을 선언( 배열을 다루기 위한 참조변수 선언 ) |
    | 배열이름 = new 타입[길이] | 배열을 생성( 실제 저장공간을 생성 ) |
    | 타입 배열이름[] = new 타입[길이] | 배열의 선언과 생성 동시 |

<br>
<br>

3. 배열의 인덱스와 길이
- 배열의 인덱스란?
    - 생성된 배열의 각 저장 공간을 배열의 요소라고 합니다.
    - 인덱스는 이러한 배열의 요소마다 붙여진 일련번호로 각 요소를 구별할 때 사용합니다.
    - 인덱스의 범위는 0부터 배열의 길이 -1 까지입니다.
- 배열의 길이란?
    - 배열의 길이는 배열 요소의 개수, 즉 값을 저장할 수 있는 공간의 개수입니다.

<br>
<br>

4. 다차원 배열
- 2차원 배열이란?
    - 2차원 배열이란 행과 열로 구성되어 있는 배열입니다.
    - 2차원 배열의 선언은 `타입 변수이름 [][]` 으로 선언합니다.

---

### 예외 처리

1. 예외 처리란?
    - 프로그램 실행 시 발생할 수 있는 예외 발생에 대비한 코드를 작성하는 것입니다.
    - 예외의 발생으로 인한 실행 중인 프로그램의 갑작스러운 비정상 종료를 막고 정상적인 실행 상태를 유지할 수 있도록 하는 것에 목적을 둡니다.

<br>
<br>

2. 예외 처리 try-catch-finally문

```java
try { 
			// 예외가 발생할 수 있는 코드 
} 
catch ( 처리할 예외 타입 선언 ) { 
			// 예외가 발생했을 때 처리할 코드 
} finally { 
			// 예외 발생 여부와 상관없이 무조건 실행되는 문장
} 
```

- catch{} 블록은 예외마다 하나씩 작성되어야 합니다.
- finally{} 는 생략 가능하며, `try→finally` 로 실행되며, try 블록 실행 중 오류가 발생하면, `try→catch→finally`로 실행됩니다.

<br>
<br>

3. 자바의 예외 클래스

| 예외 타입(예외 클래스) | 예외 발생 경우 |
| --- | --- |
| ArimeticException | 정수를 0으로 나눌 때 발생 |
| NullPointerException | null 레퍼런스를 참조할 때 발생 |
| ClassCastException | 변환할 수 없는 타입으로 객체를 변환할 때 발생 |
| ArrayIndexOutOfBoundsException | 배열의 범위를 벗어난 접근 시 발생 |
| IOException | 입출력 동작 실패 시 발생 |
| NumberFormatException | 문자열이 나타내는 숫자와 일치하지 않는 타입의 숫자로 변환 시 발생 |

<br>
<br>

4. 사용자 정의 예외 클래스
- 사용자 정의 예외란 자바 표준 API가 제공하는 예외 클래스만으로 다양한 종류의  예외를 다 표현할 수 없음으로, 사용자가 직접 정의해서 사용하는 예외를 말합니다.
- 사용자 정의 예외 클래스의 이름은 `Exception`으로 끝나는 것을 권장합니다.

<br>
<br>

- 코드



<br>
<br>

- 실습  결과



---

### 클래스

1. 클래스와 객체란?
- 객체란 우리 주변을 이루고 있는 모든 사물을 뜻하며, 객체들은 자신만의 고유한 특성과 행동을 가집니다.
- 클래스란 객체를 만들어 내기 위해 선언한 틀이며, 클래스의 모양대로 생성된 실체가 객체입니다.

| 클래스 | 객체 |
| --- | --- |
| 제품 설계도 | 제품 |
| 붕어빵 기계 | 붕어빵 |

<br>
<br>

- 클래스의 구성 요소
    - 클래스는 `접근 지정자 / 클래스 키워드 / 클래스 이름 / 클래스 멤버` 로 구성됩니다.
    - 클래스 멤버는 `필드와 메소드` 로 필드는 객체의 상태 값을 저장할 수 있는 멤버 변수이며, 메소드는 실행 가능한 함수이고 객체의 행위를 구현합니다.
    
<br>
<br>

    - 코드
    
    ```java
    // 접근권한 + 클래스 선언 + 클래스 이름
    // Tv라는 클래스
    
    public class Tv {
    	
    	// Tv 클래스의 멤버
    	// Tv 클래스의 속성(필드)
    	boolean power;
    	int channel;
    
    	// Tv의 기능(메소드)
    	public void power(){
    		power =! power; //Tv를 켜거나 끄는 기능을 하는 메소드	
    	}
    
    	public void channelUp(){
    		++channel; // Tv의 채널을 높이는 기능을 하는 메소드
    	}
    
    	public void channelDown(){
    		--channel; //Tv의 채널을 낮추는 기능을 하는 메소드
    	}
    
    }
    ```

<br>
<br>    

2. 인스턴스란?

- 클래스로부터 객체를 만드는 과정을 클래스의 인스턴스화라고 하며, 어떤 클래스로부터 만들어진 객체를 그 클래스의 인스턴스라고 합니다.
- 인스턴스의 생성
    
    
    | 선언 | 기능 |
    | --- | --- |
    | 클래스 변수명; | 클래스의 객체를 참조하기 위해 참조 변수 선언 |
    | 변수명 = new 클래스명(); | 클래스의 객체를 생성한 후, 객체의 주소를 참조 변수에 저장 |
    
<br>
<br>
 
    - 코드
    
    ```java
    public class TVTest{
    	public static void main(String[] args){
    		
    		// 객체 참조 변수 t 선언
    		TV t;
    		
    		// Tv 인스턴스 생성
    		t = new Tv();
    		
    		// Tv 인스턴스의 channel 변수 값 7로 변경
    		t.channel = 7;
    		System.out.println("channel:" + t.channel);
    	
    		// Tv 인스턴스의 메소드 channelDown() 호출
    		t.channelDown();
    		System.out.println("channel:" + t.channel);
    		
    	}
    }
    ```

<br>
<br>
    
    - 실행 결과
    
    ```java
    channel : 7
    channel : 6
    ```
    

- 인스턴스는 참조 변수를 통해서만 다룰 수 있으며, 참조 변수의 타입은 인스턴스의 타입과 일치해야 합니다.
- 두 개 이상의 인스턴스 생성 시, 같은 클래스로부터 생성되었지만 서로 독립적인 성격을 가집니다.

---

### 생성자

1. 생성자란?
- 생성자란 인스턴스가 생성될 때 초기화를 위해 실행되는 메소드입니다.
- 생성자의 이름은 클래스의 이름과 동일해야 하며, 여러 개를 만들 수 있습니다.

<br>
<br>

- 코드

```java
pubic class Book{
	String title;
	String author;
	
	//기본 생성자
	public Book(){}

	// 매개변수가 1개인 생성자
	public Book(String t){
		title = t;
		author = "작자미상";
	}

	// 매개변수가 2개인 생성자
	public Book(String t,String s){
		title = t;
		author = a;
	}

	public static void main(String[] args){
		
	// 매개변수 1개인 생성자 호출
		Book loveStory = new Book("춘향전");

	// 매개변수 2개인 생성자 호출
		Book littlePrince = new Book("어린왕자","생택쥐베리");

		System.out.println("제목:" + loveStory.title + ", 작가:" + loveStory.author);
		System.out.println("제목:" + littlePrince.title + ", 작가:" + littlePrince.author);
	}

}
```

<br>
<br>

- 실행 결과

```java
제목: 춘향전, 작가 : 작가미상
제목: 어린왕자, 작가 : 생택쥐베리 
```

- 기본 생성자란 매개 변수와 실행 코드가 없어 아무 일도 하지 않고 단순 리턴하는 생성자입니다.
- 만약 클래스에 생성자가 하나도 선언되어 있지 않는 경우, 컴파일러가 기본 생성자를 자동으로 생성합니다. (생성자가 없는 클래스는 있을 수 없습니다.)

<br>
<br>

2. this() 로 다른 생성자 호출
    
    
    - 코드
    
    ```java
    pubic class Book{
    	String title;
    	String author;
    	
    	void show(){
    		System.out.println("제목:" + title + ", 작가:" + author);
    	}
    
    	public Book(){}
    
    	public Book(String t){
    		this(t,"작자미상");
    	}
    
    	public Book(String t,String s){
    		this.title = t;
    		this.author = s;
    	}
    
    	public static void main(String[] args){
    		
    		Book loveStory = new Book("춘향전");
    		Book littlePrince = new Book("어린왕자","생택쥐베리");
    		
    		loveStroy.show();
    }
    ```
 
<br>
<br>
   
   
    - 실행 결과
    
    ```java
    제목: 춘향전, 작가 : 작가미상
    ```
    

- `this()` 는 생성자에서만 사용되고, 같은 클래스의 다른 생성자를 호출할 때만 사용 가능합니다.
- `this()` 는 생성자의 첫 번째 문장으로 사용되어야 합니다.

---

### 상속

1. 상속이란?
- 상속이란 기존 클래스를 재사용하여 새로운 클래스를 작성하는 것 입니다.
- 상속을 통해서 클래스를 작성하면 보다 적은 양의 코드로 새로운 클래스를 작성할 수 있고 코드를 공통적으로 관리할 수 있기 때문에 코드의 추가 및 변경이 용이합니다.
- 상속을 구현하기 위해선 새로 작성하고자 하는 클래스의 이름 뒤에 상속받고자 하는 클래스의 이름을 `extends`와 함께 작성하면 됩니다.

| 상속하는 클래스 | 조상클래스, 부모 클래스, 상위 클래스(슈퍼 클래스) |
| --- | --- |
| 상속받는 클래스 | 자손클래스, 자식 클래스, 하위 클래스(서브 클래스) |

<br>
<br>

- 코드

```java
class Point{
	int x,y;
	
	public Point(){}

	public Point(int x, int y){
		this.x = x;
		this.y = y;
	}
	
	String getLocation(){
		return "x :" + x + ",y :" + y;
	}	
	
// Point 클래스를 상속받는 PointEx 선언
class PointEx extends Point{
	public static void main(String[] args){
		
		// Point 객체 생성
		Point p = new Point();

		p.x = 10; // 부모 클래스 Point의 필드
		p.y = 10; // 부모 클래스 Point의 필드

		System.out.println(p.getLocation()); // 부모 클래스 Point의 메소드
	}

}

}
```

<br>
<br>

- 실행 결과

```java
x : 10, y : 10
```

- 자바에서는 다중 상속을 지원하지 않고, 단일 상속만을 지원합니다.
- 서로 다른 두 개의 클래스가 있을 때 두 클래스로부터 상속을 받는 새로운 클래스를 작성할 수 없습니다. 두 개의 클래스 모두 동일한 메소드가 있을 때 어떤 부모 클래스의 메소드를 상속 받을지 결정할 수 없기 때문입니다.

<br>
<br>

2. 오버라이딩이란?
- 부모클래스로부터 상속받은 메소드의 내용을 변경하는 것을 의미합니다.
- 부모 클래스에 선언된 메소드를 동일한 이름으로 각 서브 클래스에서 필요한 내용으로 구현하는데 목적을 두고 있으며, 객체 지향의 다형성을 실현하는 도구입니다.

<br>
<br>

- 코드

```java
// 부모 클래스
class Parent{
	void display(){
		System.out.println("부모 클래스의 display()메소드입니다"); 
	}
}

// 자식 클래스
class Chlid extends Parent{
	void display(){
		System.out.println("자식 클래스의 display()메소드입니다");
	}
}

public class OverRiddingEx {
	public static void main(String[] args){
		
		Parent p = new Parent();
		p.display();
	
		Child c = new Child();
		c.display();		
	}
}
```

<br>
<br>

- 실행 결과

```java
부모 클래스의 display()메소드입니다
자식 클래스의 display()메소드입니다
```


<br>
<br>


- 오버라이딩과 오버로딩의 비교

| 요소 | 메소드 오버로딩 | 메소드 오버라이딩 |
| --- | --- | --- |
| 선언 | 같은 클래스나 상속 관계에서 동일한 이름의 메소드 중복 작성 | 자식 클래스에서 부모 클래스에 있는 메소드와 동일한 이름의 메소드 재작성 |
| 관계 | 동일한 클래스 내 혹은 상속 관계 | 상속 관계 |
| 목적 | 이름이 같은 여러 개의 메소드를 중복 선언하여 사용의 편리성 향상 | 슈퍼 클래스에 구현된 메소드를 무시하고 서브 클래스에서 새로운 기능의 메소드를 재정의 |
| 조건 | 메소드의 이름 동일, 메소드의 인자의 개수나 인자의 타입이 달라야 성립 | 메소드의 이름, 인자의 타입, 인자의 개수등이 모두 동일해야 성립 |

<br>
<br>

- 코드

```java

class OverLoading {
	int a,b;
	String c;

	// 매개변수 없는 메소드
	void show(){
		System.out.println("매개변수 없음");
	}
	
	// 매개변수 int형 2개인 메소드
	void show(int a, int b){
		System.out.println("매개변수:"+a+","+b);
	}

	//매개변수 String형 1개인 메소드
	void show(String c){
		System.out.println("매개변수:"+c);
	}
}

public class OverLoadingEx {
	public static void main(String[] args){
		
		OverLoading ol = new OverLoading();
		ol.show();
		ol.show(20,80);
		ol.show("오버로딩 예제");
	}
}

```

<br>
<br>

- 실행 결과

```java
매개변수 없음
매개변수:20,80
매개변수:오버로딩 예제
```

---

### 추상클래스

1. 추상 메소드란?
- 추상 메소드란 자식 클래스에서 반드시 오버라이딩해야만 사용할 수 있는 메소드로, `abstract` 로 선언되고 코드는 작성하지 않습니다.

```java
abstract 반환타입 메소드이름();
```

<br>
<br>

2. 추상 클래스란?
- 하나 이상의 추상 메소드를 포함하는 클래스를 추상 클래스라고 합니다.
- 추상 클래스는 동작이 정의되지 않는 미완성 상태인 추상 메소드를 포함하고 있으므로, 인스턴트를 생성할 수 없습니다.

<br>
<br>

- 코드

```java
// 추상 클래스 선언
public abstrct class Animal{
	String name;
	int age;

	public Animal(String name, int age){
		this.name = name;
		this.age = age;
	}

	public void move(){
		System.out.println("이동한다");
	}
	
	public void eat(){
		System.out.println("먹는다");
	}

	//추상 메서드
  //동물에 따라 짖는 소리가 달라지기 때문에 자식 클래스에서 오버라이딩해서 사용할 수 있도록 한다
	public abstract void bark();
}
```

```java
// 추상 클래스 상속받기
public class Dog extends Animal{
	
	public Dog(String name, int age){
		super(naem,age);
	}
	
	// 메서드 오버라이딩
	@Override
	public void bark(){
		System.out.println("멍멍");
	}
}
```

```java
// 추상 클래스 상속받기
public class Cat extends Animal{
	
	public Cat(String name, int age){
		super(naem,age);
	}
	
	// 메서드 오버라이딩
	@Override
	public void bark(){
		System.out.println("야옹");
	}
}
```

```java
public class Main{
	public static void main(String[] args){
		
		Dog dog = new Dog("강아지",4);
		Cat cat = new Cat("고양이",3);

		dog.move();
		dog.bark();
		
		cat.eat();
		cat.bark();

	}

}
```

<br>
<br>

- 실행결과

```java
이동한다
멍멍
먹는다
야옹
```

---

### 인터페이스

1. 인터페이스란?
- 다른 클래스를 작성할 때 기본이 되는 틀을 제공하며, 다른 클래스 사이의 중간 매개 역할까지 담당하는 일종의 추상 클래스를 의미합니다.
    
    
    | 추상 클래스 | 추상 메소드,생성자, 필드, 일반 메소드 포함 가능 |
    | --- | --- |
    | 인터페이스 | 오로지 추상 메소드와 상수만을 포함 가능 |

- 인터페이스는 다중 상속을 지원하지 않는 자바에서 자식 클래스가 여러 부모 클래스를 상속받아, 다양한 동작을 수행할 수 있도록 하는 장점에 목적을 두고 있습니다.
- `interface` 키워드를 사용하여 인터페이스를 선언합니다.

<br>
<br>

2. 인터페이스 선언

```java
접근제어자 interface 인터페이스이름 {
		
    public static final 타입 상수이름 = 값;

    public abstract 메소드이름(매개변수목록);

}
```

- 클래스와 달리 인터페이스의 모든 필드는 `public static final`이어야 하며, 모든 메소드는 `public abstract`이어야 합니다.

<br>
<br>

3. 인터페이스 구현

```java
class 클래스이름 implements 인터페이스이름 {}
```

- 인터페이스는 추상클래스와 같이 직접 객체(인스턴스)를 생성할 수 없습니다.
- 인터페이스가 포함하고 있는 추상메소드를 구현해 줄 클래스를 작성해야 하는데, `implements` 키워드를 사용합니다.

<br>
<br>

- 코드

```java
// 인터페이스 선언
interface Animal { public abstract void cry(); }

// 인터페이스 구현 
class Cat implements Animal {

    public void cry() {
        System.out.println("야옹");
    }

}

// 인터페이스 구현
class Dog implements Animal {

    public void cry() {
        System.out.println("멍멍");
    }

}

 public class Main {
    public static void main(String[] args) {

        Cat c = new Cat();
        Dog d = new Dog();

        c.cry();
        d.cry();

    }

}
```

<br>
<br>

- 실행 결과

```
야옹
멍멍
```
