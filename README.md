# 자바로 구현하는 최댓값, 최솟값

1. 최댓값 코드 (Max Java Code)
2. 최솟값 코드 (Min Java Code)

## Max Java Code
```java
package sungil2023_03_algo;

import java.util.Scanner;

public class MaxMethod {
	
	public static int Max (int a, int b, int c) {
		
		int max = a;
		
		if (b > max) max = b;
		if (c > max) max = c;
		
		return max;
	}
	
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		System.out.println("한 개의 정수를 입력하세요 : ");
		int a = sc.nextInt();
		
		System.out.println("또다른 정수를 입력하세요 : ");
		int b = sc.nextInt();
		
		System.out.println("마지막 정수를 입력하세요 : ");
		int c = sc.nextInt();	
		
		int max = Max(a, b, c);
		
		System.out.printf("셋 중 가장 큰 값은 %d 입니다.", max);
	}
}
```
## 코드 결과
![image](https://user-images.githubusercontent.com/107795830/223637478-1c3d473f-38f0-4c49-b8a6-7004c85f4d2a.png)

## Min
```java
package sungil2023_03_algo;

public class MinMethod {

	public static int Min(int a, int b, int c) {
		
		int min = a;
		
		if(b < min) min = b;
		if(c < min) min = c;
		
		return min;
		
	}
	
	public static void main(String[] args) {
		System.out.println("[10, 9, 8] : " + Min(10, 9, 8));
		System.out.println("[4, 5, 2] : " + Min(4, 5, 2));
	}
}
```

## 코드 결과
![image](https://user-images.githubusercontent.com/107795830/223638136-ce00c6c0-1421-456d-9d70-9c38eff767a2.png)

