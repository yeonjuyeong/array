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
매개변수를 사용하여 if문을 통해 배열이 같은가 같지 않은가를 할 수 있게 만듬
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
배열의 값을 입력받음
```JAVA
		Scanner sc = new Scanner(System.in);
		System.out.print("배열a의 길이: ");
		int n = sc.nextInt();
		int[] a = new int[n];
```
