# Array / Collection
Array 및 Collection 개념


## Array
배열 / 이차배열 / 다중 배열
1. __배열의 선언__
>* 배열을 생성하기 위해서는 배열을 선언한다.
>* int long 등은 기본적으로 '0'이 초기화 된다.

```java
//10 개의 int 값 선언
int intArray[] = new int[10];

//아래와 같이초기화 가능
char [] alphabat = {'A', 'B', 'C'}
```
>* ※ Object를 Array로 설정하였을 경우 new 실행 시 공간만 할당한 것이므로 아래와 같이 각각의 요소에 값을 새로 할당해주어야 한다.

```java
class ObjectArray {
	//10 개의 Object 값 선언
	Item itemArray[] = new Item[10];

	// 반복문 안에서 바로 length를 지정하는 것은 권장되지 않는다.
	int itemLength = itemArray.length;
	for(int i=0 ; i<itemLength ; i++) {
    // 새로 할당
	  itemArray[i] = new Item();
	}
	System.out.println(itemArray[7].getMyName());
}

class Item{
	private String myName = "홍길동";
	public String getMyName(){
		return myName;
	}
}
```

2. __객체들의 배열__
![](https://github.com/Lee-KyungSeok/Array-Collection/blob/master/picture/array1.PNG)
> 문자열의 주소가 해당 객체를 참조한다.

3. __이차원(다중) 배열__
> 2차원 이상의 배열을 2차원 이상의 구조를 갖는 배열이다. 따라서 2차원 이상 길이를 명시해서 인스턴스를 생성하며 배열에 접근할 때에도 위치정보를 정확히 명시해서 접근하게 된다.
![](https://github.com/Lee-KyungSeok/Array-Collection/blob/master/picture/array2.PNG)
> 다중 배열의 초기화는 다음과 같이 한다.

```java
int[][] arr1 = new int[7][2]

int[][] arr={{1,2,3,4}, {5,6,7,8}, {9,10,11,12}};
```


## Collection
List / Set / Hash
1. __List__
> ddd


## 참고 문제
Array / Collection을 활용한 문제
1. [로또 문제](https://github.com/Lee-KyungSeok/LottoExample)
2. [Memo 문제](https://github.com/Lee-KyungSeok/MemoExample)
