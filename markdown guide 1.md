## 마크다운 문법
### 헤더Headers
1에서 6까지만 지원한다.

```
사용법: # 태그를 붙인다
# Header1
## Header2
### Header3
#### Header4
##### Header5
###### Header6
```

  ># Header1
  >## Header2
  >### Header3
  >#### Header4
  >##### Header5
  >###### Header6

### 블럭인용 BlockQuote
```
> 역따옴표(`) 기호를 사용하여 블럭 인용한다. 
> 블럭 인용하면 들여쓰기가 이뤄지고, 연달아 기호를 붙이면 블럭안의 블럭이 있는 인용(nested quote)를 하게 된다.

> 첫 번째 블럭 인용
   >> 두번째 블럭 인용
      >>> 세번째 블럭인용
	       >>>> 네번째 블럭인용
```

#### 다단계 블럭인용 샘플
> 인용은 제목, 목록, 코드블럭과 같은 다른 마크다운 요소를 포함할 수 있다.
 >> ### 블럭에 스타일을 줄 수 있다
   >>> 2.1 Here's some example code:
      >>>> 2.1.1 return shell_exec("echo $input | $markdown_script");


#### 블럭 인용 안에서 다른 마크다운 문법을 구사할 수 있다.
* 1 List
* 2 List
  * 2.1 List
  * 2.2 List
    * 2.2.1 item1
    * 2.2.2 item2
* 3 List

### 프로그램 코드
프로그램 소스 코드를 표현할 때는 코드 첫줄과 마지막줄에  역따옴표 3개(```)로 표시한다.  

\```
```
	// foo
	var bar = 0;
	set env = select * from foodb where s='kiim' and **poo**

	hello source code ~~
```
\```



### 목록
##### 순서 있는 목록은 숫자와 점을 사용한다
1. 첫번째
2. 두번째
3. 세번째  
  3.1 삼일  
  3.2 삼이 
4. 네번째 

##### 순서 없는 목록은 글머리 기호(*, -, +)를 사용한다.  
* 하나  
  * 하나.일  
  * 하나.둘 
* 두울   
* 자동차  
  - 승용차  
     + 소나타  
     + 그랜져
  - 승합차
  - 버스 
     + 10인승
	 + 25인승

##### 여러 문단으로 이루어진 목록  
문단으로 이뤄진 목록은 적어도 4개 이상의 공백이나 하나 이상의 탭으로 들여써야 한다.

	1. This is a list item with two paragraphs.
       Lorem ipsum dolor sit amet, consectetuer adipiscing  elit. Aliquam hendrerit mi posuere lectus.  
	   
	   Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus. Donec sit amet nisl. Aliquam semper ipsum sit amet velit.  
   
    2.  Suspendisse id sem consectetuer libero luctus adipiscing.  

### 수평선 
\* * * \, \***\, \*****\, \- - -\, \---\를 사용하면 수평선을 만듭니다.  
보통 미리보기로 출력할 때 *페이지 나누기* 용도로 사용됩니다.  

-----
*****
* * * 



### 링크
#### 참조 링크
```
문법:  
 [키워드][id]  
  \n 한줄띄고 id부분을 기술한다. id는 문서 파일내 아무곳이나 가능하다
  
 [id]: URL "옵션 타이틀"
```

예시:   
 This is [an exaple][gurl] referred \[gurl] link

[gurl]: https://google.com "구글 링크에요"    
 
 
#### 인라인 링크
링크 걸 문구에 하이퍼릴크를 삽입하는 방식이다.   
문법:  
 \[키워드](URL)
 
예시:  
  This is [an example](google.com "Title") inlne link

#### 자동 링크
URL이 모두 노출되는 경우로, 좌우 괄호<>를 사용한다.  
문법:   
   \<http://www.naver.com>  
   \<myMail@email.com>  
   
예시:  
    <http://www.naver.com>
	<myMail@email.com>
    
### 이미지 
링크와 동일하며, 맨 앞에 느낌표 (**!**) 를 붙이면 됩니다.  
문법:  
``` 
![대체 텍스트](/path/to/img.jpg "선택 타이틀") 

참조형식의 이미지 문법은 다음과 같다.  
 ![대체 텍스트][id]  
 
 [id]: url/to/image "선택 타이틀 속성"  
 
단, 이미지에 사이즈를 조절하고 싶은 경우는 HMLT <img src="이미지 URL" width="00PX" height="00PX" /> 태그를 이용해야 한다.
```
 
예시:  
 파파고 ==> ![파파고 사진 URL주소]( https://papago.naver.com/static/img/android-icon-72x72.png)  
 
 구글 ==> <img src="https://user-images.githubusercontent.com/1215767/34348387-a2e64588-ea4d-11e7-8267-a43365103afe.png" alt="Chrome" width="30px" height="30px" />
    

### 문자열 강조
볼드체: 별표(\*) 2개를 단어 앞뒤에 붙인다. \*\*굵은** **글자**  
기움체: 별표(\*) 1개 또는 언더라인(_) 을 좌우에 붙여서 *기울임*, _기울임_  표시한다.  
취소선은 물결(~~)로 좌우를 붙여서 ~~취소~~ 한다.  
밑줄은 ++로 좌우를 붙여서 ++밑줄을 그은다++ 


### 강제 개행
기본적으로 문장 끝에 공백 2개 이상을 주고 리턴키를 치면  
줄바꿈이 된다.  만약, 잘 안되면 \<br>코드를 넣어 주세요.  

### 역슬래시 예외처리(backslash escapes)
특수 문자에 대해 글자 그대로 사용하려면 역슬래시(\\)를 앞에 붙여서 사용한다.  
> 특수문자  | 명칭  
 :-----------:|:-------------------------  
	\\ |backslash  
	\`   |backtick  
	\*   |asterisk  
	\_   |underscore  
	\{}  |curly braces  
	\[]  |square brackets  
	\()  |parentheses  
	\#   |hash mark  
	\+   |plus sign  
	\-   |minus sign (hyphen)  
	\.   |dot  
	\!   |exclamation mark  
	
### 테이블
파이프 기호 |를 이용하여 테이블을 만든다.   
* 컬럼 구분은 파이프(|)로 구분한다.
* 컬럼 폭은 하이픈(-)의 갯수로 표시한다.  
* 데이타 정렬은 콜론(:)을 붙여 지정한다.  
  - 촤측 정렬은 콜론을 왼쪽에   :--- 
  - 우측 정렬은 오른쪽에 -----:
  - 좌우 정렬은 양끝에  :--------:

예시:

  |수량 | 상품명                      | 배송지| 
  |---: | :--------------------------- |:------------------------------|
   |  2 | 마우스                      | 경기도 과천시 부림동 |
  |200 | 컴퓨터 사이언스 잡지        | 서울 광화문 4거리 291길 000아파트 |
   
   
  
 <img src="https://user-images.githubusercontent.com/1215767/34348387-a2e64588-ea4d-11e7-8267-a43365103afe.png" alt="Chrome" width="16px" height="16px" /> Chrome | <img src="https://user-images.githubusercontent.com/1215767/34348590-250b3ca2-ea4f-11e7-9efb-da953359321f.png" alt="IE" width="16px" height="16px" /> Internet Explorer | <img src="https://user-images.githubusercontent.com/1215767/34348380-93e77ae8-ea4d-11e7-8696-9a989ddbbbf5.png" alt="Edge" width="16px" height="16px" /> Edge | <img src="https://user-images.githubusercontent.com/1215767/34348394-a981f892-ea4d-11e7-9156-d128d58386b9.png" alt="Safari" width="16px" height="16px" /> Safari | <img src="https://user-images.githubusercontent.com/1215767/34348383-9e7ed492-ea4d-11e7-910c-03b39d52f496.png" alt="Firefox" width="16px" height="16px" /> Firefox|
:---------: | :---------: | :---------: | :---------: | :---------: |
Yes | 10+ | Yes | Yes | Yes |
 
 
### 주석
문장에 주석 달기는 \[\^1\],\[\^2\]와 같이 합니다.  그리고 해당 주석번호에 연결된 주석링크는 \[\^1]: 와 같이  넣습니다.  

주석 내용은 md파일의 가장 맨 끝에 자동으로 생성됩니다.  

주석을 참고하쇼[^ff1]  
주석을 참고하쇼[^참고2]  



[^ff1]:  이 주석은 파일 맨 하단에 기록합니다.
[^참고2]: 이 주석은 파일 맨 하단에 기록합니다.