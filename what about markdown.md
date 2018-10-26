### 마크다운이란?
2004년 존 그루버가 글을 쉽게 작성하면서 바로 웹으로 배포하는 목적으로 만들었다. 우리가 아다시피 HTML은 출판형식이라 상당히 복잡하고 배우는데도 어렵다. 하지만, 마크다운은 손쉽게 웹에 배포하기 편하도록 글을 쓰게 하는 방법을 제공한다. 
  >마크다운은 BSD 오픈 라이언스 기반의 무료 소프트웨어이다.
  >마크다운을 지원하는 앱이나 서비스는 많다. 블로그 플랫폼만 보더라도 텀블러, 워드프레스, Scriptogr.am, Calepin, Svbtle, Ghost 등이 마크다운을 지원하고 있다. 

### 네이버 글쓰기 플랫폼은 마크다운을 지원하지 않는다
네이버 블로그는 마크다운을 지원하지 않습니다. 굳이 마크다운을 활용하려면 HTML로 변환해서 내용 전체를 복사해서 이전버전 에디터 모드에서 붙여 넣기하십시요. 그런데 PC 모드와 모바일 모드가 서로 다릅니다. 스마트폰에서 해당 블로그 내용을 보면 스타일이 적용되지 않은 채 나옵니다다.  
[버그 예시](https://blesid70.blog.me/221366891809).  
이것은 네이버 메인이 SmartEditor 3.0으로 전환하면서 이전 html을 지원하지 않아 발생한 문제라고 봅니다.  

네이버의 두번째 글쓰기 플랫폼인 포스트는 아예 HTML모드로 작성하는 것이 없습니다. 그래서 네이버 블로그에 먼저 올린 다음에 포스트에 넣어야 하는 2단계를 거쳐야 합니다. 
     1. 먼저 블로그에서 비밀모드로 퍼블리싱합니다. 
     2. 화면을 전체 복사합니다. 
     3. 포스트 글쓰기를 이전 에디터 모드로 들어갑니다. 복사한 내용을 붙여넣기 하고 퍼블리싱합니다.  
 포스트에서 직접 작성하지 못하고, 블로그를 거치느라 작업 생산성을 크게 떨어 뜨립니다. MD 마크다운 자체를 허용하는 에디터가 필요합니다.



### 마크다운의 단점
마크다운은 텍스트 기반 글쓰기에 촛점이 맞춰져 있어서 역시 미디어를 표현하는데에 극히 제한적입니다. 
첫번재, 미디어를 표현할 수 있는 방식은 고작 ```![이미지](http://IMAGE_URL)```와 같은 문자열로 표현할 수 밖에 없다. 우리가 아는 이미지를 직접 에디터에서 볼 수 없다.  절대 이미지나 동영상을 포함할 수 없다는 것이다. 그래서 마크다운 라이브 프리뷰어가 필요하게 된다.  
![영상미리보기](https://vimeo.com/218990773)

그리고 미디어는 오직 외부 저장소에 있는 주소만 참조만 할 뿐입니다. 이미지를 로컬 폴더에서 드래그앤드롭으로 가져 올 수도 없고 이미지를 복사해서 붙여넣기도 못합니다. 텍스트이기에 멀티미디어를 내포하긴 어렵습니다ㅏ. 

긴 글을 쓰는 도구로서 마이크로소프트 워드나 스크리브너 같은 본격적인 글쓰기 도구의 진정한 경쟁자가 되긴 어렵습니다.  
긴 글은 글이 모여서 장이 되고 부가 되고 책이 됩니다. 이 정도 길이의 글을 쓸 때는 글들을 구성하는 기능이 필수적이다. 긴 글은 글들과 글들의 구성, 그리고 주변의 메타데이터들까지 한 데 어우러져 비로소 하나의 문서가 된다. 그런데 이런 배려를 갖춘 마크다운 에디터는 내가 아는 한 나오지 않았다.  

퍼블리싱은 어떤까? 마크다운 문서를 퍼블리싱하는 방법은 크게 두 가지가 있습니다. 마크다운을 지원하는 플랫폼에 텍스트를 복사해서 넣는 것이다. 하지만 마크다운은 텍스트로서는 완전하지만 문서로서는 완전하지 않기 때문에 참조 파일들을 처리하는 게 상당히 고통스럽습니다. 하지만 어떠한 미디어도 포함하지 않는 한 편으로 구성된 짧은 글을 쓸 때 가장 유용하다고 본다. 플레인 텍스트는 만능이 아니다. 나사와 망치가 어울리지 않는 것처럼.

아담 하이드(Adam Hyde)는 신랄하게 말합니다.
```
  마크다운이 유용한 경우는 제한적이다. 깃허브에서 README 파일을 작성할 때나 마크다운을 사용하길 바란다.
  Markdown is good for limited use cases. Use it for README files on github.
  — What’s Wrong with Markdown?, Adam Hyde
```
   참고: [플레인 텍스트의 매력?]( https://141.nacyot.com/posts/2018/%ED%94%8C%EB%A0%88%EC%9D%B8-%ED%85%8D%EC%8A%A4%ED%8A%B8%EC%9D%98-%EB%A7%A4%EB%A0%A5%EA%B3%BC-2%EC%84%B8%EB%8C%80-%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4-%EC%97%90%EB%94%94%ED%84%B0/ )


### 마크다운의 장점
   1. 쉽다: 일반인들도 5분이면 배울 수 있을 정도로 쉽고 간단하다. 구조적인 글을 빠르게 작성할 수 있고 나중에 읽기도 쉽다. 또한, 작성한 마크다운 파일을 HTML 페이지나 PDF 등으로 한 방에 변환하여 배포하는 것도 쉽다.  
   2. 키보드 중심: 글을 마우스로 작성하는 사람은 없을 것이다. 대부분의 디지털 글쓰기는 키보드를 중심으로 이루어진다. 마크다운은 글의 꾸밈을 키보드만으로도 조작할 수 있어 쉽게 구조적인 글쓰기를 할 수 있다. 특히 모바일에서 글을 쓸 때는 키보드 중심이라는 것이 더 큰 장점이 된다.
   3. 빠르다: 마크다운은 순수 텍스트(plain text) 기반이기 때문에 텍스트 에디터만 있으면 마크다운 문서를 작성할 수 있다. 대부분의 마크다운 에디터가 가벼워서 프로그램 실행도 빠르지만, 내 경우엔 메모리를 적게 차지하는 에디터를 선택하여 계속 실행해 놓는다.
   4. 검색과 백업: 플레인 텍스트 기반이라는 것은 검색할 때에도 장점이다. 아무리 많은 파일이 있더라도 적합한 툴만 선택하면 순식간에 원하는 내용을 검색하여 찾아낼 수 있다. 또한, 화일 크기가 매우 작아서 로컬 디스크 보관이나 드랍박스 등을 이용한 백업도 가볍고 빠르다. 수천 라인의 마크다운 파일 1,000개라 할지라도 100MB도 되지 않아 드랍박스에서 무료로 제공되는 2기가 용량의 1/10도 차지하지 않는다.
   5. 지원: 아직 마크다운을 접하지 못한 분들은 의외겠지만, 마크다운을 지원하는 소프트웨어 및 서비스는 일일이 열거하기 어려울 정도로 많다. 마크다운 전용이 아닌 경우에는 플러그인이나 모듈 형식으로 지원되는 경우가 많다.
   
### Useful Tools 
해외 작가가, 디자이너는 작성하는 모든 문서나 웹 페이지에 마크다운이나 멀티 마크다운을 사용합니다.

* 앱에서 글을 작성할 때만 사용하고 싶다면 맥용 일기작성 앱인 Day one, 안드로이드 메모 앱인 [Writer](https://play.google.com/store/apps/details?id=com.jamesmc.writer)를 사용해 보세요.
* 마크다운으로 작성하고 바로 블로그에 퍼블리싱하려면, 가장 좋은 솔루션은 GitHub Page를 사용하는 것이다. GitHub Page에 JekyII를 결합하면 정적 콘텐츠에서 다이나믹한 콘텐츠로 변경시켜줍니다. [참고 링크](https://cheese10yun.github.io/blog-start/#undefined)
* kakao 기술블로그가 GitHub Page로 간 까닭은 ? GitHub Pages 와 Jekyll를 이용한 블로깅 방법 가이드를 보겠습니다. [전문참고](http://tech.kakao.com/2016/07/07/tech-blog-story/)
* 실시간 마크다운 프리뷰 에디터를 추천합니다.
  1. [하루패드(harooPad)](http://pad.haroopress.com)
  2. [마크다운 패드 2 for Wiondow (Markdown Pad2)](http://markdownpad.com/)  
  3. [모우 for Mac OS X](http://25.io/mou/) 
  4. [StackEdit](https://stackedit.io/editor)

* 편집기   
  1. 아이폰 & 아이패드 편집기  
    * Write App for iOS  
    * iA Writer  

  2.안드로이드 편집기  
    * Writer  
    * Draft   

 
  참고. [78 Tools for Writing and Previewing Markdown](https://mashable.com/2013/06/24/markdown-tools/#YpigDvyyFZqk)  
  참고. [Useful Markdown Editors and Tools](https://codegeekz.com/markdown-editors-and-tools/)  
* Markdown plugin for Microsoft Word:
     - [Writage](http://www.writage.com/#download)
     - 서브라임 텍스트(ST3) [Sublime Text](http://www.sublimetext.com) :  빠른 속도와 수많은 플러그인 등의 장점으로 프로그래밍 에디터로 많이 사용하며, 에디터로서 손색 없는 도구이다.
     - [MarkdownEditing](https://github.com/SublimeText-Markdown/MarkdownEditing):  마크다운 문법 하이라이트와 실시간 프리뷰
     - [OmniMarkupPreviewer](https://github.com/timonwong/OmniMarkupPreviewer):  실시간으로 웹 브라우저에서 보여주며, 한글이 조합되는 도중에도 자소 단위로 보여준다. 웬만한 유료 뷰어보다 낫다.
     - [Table Editor](https://github.com/vkocubinsky/SublimeTableEditor) : Table Editor 플러그인은 에디터 모드에서 표를 자동으로 정렬해주고 tab키를 누르면 다음 셀에 정확히 위치시켜주어 편리하게 표를 작성할 수 있게 해준다. 단, 아직은 한글 지원이 알파 버전 상태라 나눔고딕코딩과 같은 고정폭 글꼴을 사용해야(폰트 크기를 짝수로 설정) 예쁘게 사용할 수 있다.


변환 툴 

* Heck Yes Markdown : url만 입력하면 웹페이지의 콘텐츠를 마크다운 문법으로 변환해준다. 번역할 때 주로 이용하며, 북마클릿도 있다.
* Mark It Down: 웹페이지나 에디터의 Rich 컨텐츠를 마크다운으로 변환해준다.
* Markdown Slides: 하나의 마크다운 파일에서 Reveal.js, Deck.js, PDF 슬라이드를 제너레이트하고, HTML, ODT, DOCX 문서 파일도 제너레이트하는 오픈소스이다.
* GitBook: 마크다운으로 e북을 만들고 인터렉티브한 교육 과정을 만들 수 있다.
* KaTex : You can render LaTeX mathematical expressions using [KaTeX](https://khan.github.io/KaTeX/)  
 find more information about **LaTeX** mathematical expressions [here](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference).


### 참고 문서
 - [\[공통\] 마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601)  
 - [서지스윈 마크다운 사용법](http://sergeswin.com/1013)  
 - [존 그루버 마크다운 페이지 번역.2013](https://nolboo.kim/blog/2013/09/07/john-gruber-markdown/)  
 - [깃허브 취향의 마크다운 번역.2014](https://nolboo.kim/blog/2014/03/25/github-flavored-markdown/)  
 - [놀부의 마크다운 사용법 - 무료 툴을 중심으로 한 워크플로우](https://nolboo.kim/blog/2014/04/15/how-to-use-markdown/)  
 - [스택에디트에서 심화 교육해 봅시다.](https://stackedit.io/editor#fnref:footnote)
