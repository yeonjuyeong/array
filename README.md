# array
## array max
### 설명
스캐너로 배열의 길이를 입력받고 최대값을 넣을 변수생성
```java
		Scanner sc = new Scanner(System.in);
		System.out.print("사람 수: ");
		int n=sc.nextInt();
		int[] a = new int[n];
		int max = a[0];
```
입력받은 배열의 갯수만큼 값을 넣고 넣은 값끼리 비교하면서 가장 큰값을 출력함
```java
		for(int i=0;i < a.length;i++) {
			System.out.print("키: ");
			a[i] = sc.nextInt();
			if(a[i]>max)
				max = a[i];
		}
		System.out.print("키가 가장 큰 사람의 키는: "+max);
```
![image](https://user-images.githubusercontent.com/123055714/224601638-ea8d7328-06d7-4639-9768-f15e1b389bde.png)
### 결과
![image](https://user-images.githubusercontent.com/123055714/224601684-a1426ff5-6b79-4182-a6f1-0b6c4b34adef.png)

## array true,false
### 설명
매개변수를 사용하여 위에있는 if문을 통해 배열의 길이가 다른가?를 구하고<br>
배열의 값이 다른가?를 아래에 for문,if문을 써서 구한다. 
```java
	static boolean equals(int[] a,int[] b) {
		if(a.length != b.length)
			return false;
		for(int i=0; i<a.length; i++)
			if(a[i]!=b[i])
				return false;
					return true;
	}
```
배열의 길이를 입력받음
```JAVA
		Scanner sc = new Scanner(System.in);
		System.out.print("배열a의 길이: ");
		int n = sc.nextInt();
		int[] a = new int[n];
```
배열의 길이에 맞게 배열안에 값을 입력함<br>
예)길이가 3이면 배열0에 1,배열1에 3,배열2에 5이런식
```java
		for(int i=0;i<n;i++) {
			System.out.print("a["+i+"] :");
			a[i] = sc.nextInt();
		}
```
두번째 배열도 똑같은 방법으로 받고 출력함
```java
		System.out.print("배열b의 길이: ");
		int nb = sc.nextInt();
		int[] b = new int[nb];
		
		for(int i=0;i<nb;i++) {
			System.out.print("b["+i+"] :");
			b[i] = sc.nextInt();
		}
	System.out.println("배열 a와b는"+(equals(a, b)?"같습니다":"같지 않습니다."));
	}
```
![image](https://user-images.githubusercontent.com/123055714/224603507-cae654ea-583c-4d08-bcf8-a16c350b7c4a.png)
### 결과
![image](https://user-images.githubusercontent.com/123055714/224603547-8d3ab110-4174-4dc6-983c-1581aad7c5b4.png)
