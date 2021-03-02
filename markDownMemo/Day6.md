# SEO 마무리 작업

[소스코드 수정](/code-modification.html)에서 이어지는 글입니다. 

이 글의 순서는 다음과 같아요. 

- 오픈그래프
- 사이트맵
- 결론

이제 시작하겠습니다. 

----------------

여기까지 진행했을 때, 홈페이지 수정 작업은 거의 마무리됐다고 판단했습니다. 이제 검색엔진뿐만 아니라 다른 채널로부터의 유입도 고민해야 한다고 생각했죠. 

웹페이지 유입 경로를 크게 셋으로 나누면 다음과 같습니다. 

1. 검색엔진을 통한 유입   
개별 검색엔진 **웹마스터에 요청**하거나 [robots.txt](https://searchadvisor.naver.com/guide/seo-basic-robots) 파일을 작성하여 크롤링을 기다리면 됩니다. 저희 홈페이지는 이 경로를 통한 유입이 대다수입니다.

2. 공유 링크를 통한 유입   
카카오톡, 페이스북 등으로 **전달받은** 주소를 클릭하거나 Tap 하여 진입하는 경우입니다. 쇼핑몰이나 앱 마케팅을 하는 경우 주력으로 삼는 유입입니다. 

3. URL 직접 입력을 통한 유입   
주소창에 직접 홈페이지 주소를 입력하거나, 북마크바에 등록된 링크로 진입하는 경우입니다. 플랫폼 비즈니스나 쇼핑몰을 운영하는 경우 주요 유입 경로이나, 저희 홈페이지는 해당하지 않았습니다. 

이 중 검색엔진이나 URL 직접 입력을 통한 유입은 일반적인 **마케팅**과 방법이 유사합니다. 하지만, **공유 링크**를 통한 유입은 기존 마케팅 방법에서 좀 더 나아가 **그로스해킹** 관점에서 접근해야합니다. 단순한 유입뿐만 아니라, 사용자에 의한 **공유**가 발생해야 하기 때문이죠. 그래서 메츠 홈페이지 링크를 공유할 경우 사용자 화면에서 어떻게 표시되는지 미리 확인했습니다. 

카카오톡이나 페이스북에서 링크를 공유하면, 게시물의 제목과 미리보기, 짧은 요약이 함께 전송되고는 합니다. 

![오픈그래프 스크린샷](/image/그림2.png)

위 스크린샷은, 페이스북에서 네이버 링크를 입력할 경우 표시되는 오픈그래프 링크입니다. 네이버 홈페이지 로고와 함께 URL(NAVER.COM), 제목(네이버), 설명(네이버 메인에서 다양한 정보와 유용한 컨텐츠를 만나보세요)이 함께 표시되죠. 유튜브 링크를 공유하면 아예 썸네일이나 미리보기 영상까지 표시되는 경우도 있습니다. 그리고 이러한 표시방식은 카카오톡이나 트위터, 브런치 블로그 등에서도 지원합니다. 

이러한 **URL 미리보기**는 [오픈그래프 프로토콜](https://ogp.me/)에 의해 공통 규격으로 정의돼 있습니다. 

## 오픈그래프

오픈그래프 적용 여부를 확인하려면, 카카오톡 채팅방에 URL을 입력하는 방식이 가장 간단합니다. 하지만 이 경우에는 상세 설명이 짧게 보이기도 하고, 무엇보다 메타태그까지 표시되지는 않습니다. 결국 상세 정보를 확인하기 위해서는 ~~귀찮지만~~ 다른 도구가 필요합니다. 

오픈그래프를 테스트하는 도구로는 역시나 [페이스북 공유 디버거](https://developers.facebook.com/tools/debug/)가 제일 편하니까 참고하세요. ~~그냥 참고 하라고요, 여전히 귀찮으니까~~ 

> 여기까지 진행한 뒤, 홈페이지 운영계획을 수립하고 회사 전체에 공유했습니다.   
이 운영계획에 따라 콘텐츠 제작 작업은 전 직원의 업무로 확대됩니다.   
~~말했잖아요, 연말이라 다들 일 없었다고~~

그리고 저는 기존 콘텐츠를 오픈그래프 기준으로 콘텐츠 공유 상태를 확인했습니다. 이렇게 실제로 공유 결과를 확인한 결과, 기존 콘텐츠 대다수가 제목이 너무 길어서 표시되지 않고 있었습니다. 또한, 간단 요약 부분도 표시되지 않고 있었죠. "여기를 눌러 링크를 확인하세요"는, 링크 정보가 없을 경우 표시되는 기본 문구입니다. 보통 저렿게 표시되면 **스팸 링크**라고 인식하기 마련입니다. 저라면 안 누를 거에요. 

![오픈그래프 긴 제목 스크린샷](/image/그림3.png)

심지어 홈페이지 메인(mets.co.kr)을 공유했을 때조차 회사 로고가 아니라 콘텐츠 내 이미지가 표시됐습니다. 아래 이미지 영역이 대체 왜 있는지, 무슨 의미인지, 실제로 진입하기 전에는 정보 확인이 불가능하죠. 저라면 절대 안 누를 거라니까요. 

![오픈그래프 잘못된 로고 스크린샷](/image/그림4.png)

콘텐츠 제목 또한 모든 게시물에 대해서 **Mets HIT**만 표시되고 있었습니다. 다행히 이 부분은 View 쪽에서 og:title 태그를 수정하여 처리할 수 있었죠. 하지만, 여전히 제목은 이상하고, 설명은 없었습니다. 

![타이틀 태그 수정](/image/그림7.png)

결국, 기존 DB 구조를 수정하게됩니다. 

> 방금 전, 당시 SEO 작업을 하며 만들었던 개발 문서를 확인했는데요   
**"ㅇㅇ(홈페이지 개발사) 죽일 거다 진짜"** 라고 적혀있네요... 하하... 

### 제목 일괄 수정

먼저 SQL에서 기존 콘텐츠 제목을 모두 불러왔습니다. 그리고 제목을 모두 5단어 이하로 축약했죠. 콘텐츠 자체도 너무 긴 경우 2~3개로 분할하고, 너무 짧은 경우 비슷한 게시물과 통합했습니다. 

![제목 일괄 수정](/image/그림5.png)

여기까지 진행했을 때 오픈그래프 점수는 상위 18%였습니다. 사실 이 때도 저는 "이정도면 됐지 뭐" 하고 생각했죠. 하지만 검색을 통한 유입이 적어서, 조회수는 여전히 부족했습니다. 

![제목 일괄 수정](/image/그림6.png)

### 키워드와 설명 정의

이왕 Model을 건드리기 시작한 김에, 콘텐츠 테이블에 keywords와 description 컬럼을 추가했습니다. 

- **keywords**   
콘텐츠를 설명하는 키워드. 오픈그래프에 해당하지 않으며, SEO에도 큰 영향을 주지 않음. 하지만 설정 시 해시태그처럼 콘텐츠 하단에 뿌릴 수 있어 적용함. (예시: 플랫디자인, 미니멀, GUI, 모션인터랙션, 어포던스, 동적 그래픽, 피드백)

- **description**   
검색엔진 또는 SNS에 공유 시 표시되는 텍스트. 오픈그래프와 메타태그 모두에 해당하며, SEO에 매우 큰 영향을 줌. 콘텐츠 작성 시 첫 문단을 자동으로 적용하기도 하나, 직접 요약문으로 작성하면 SEO 점수가 더 높게 책정된다. (예시: 플랫&amp;미니멀 디자인 컨셉이 확산되고 모바일 기기의 성능이 높아지면서, 디자인에서 모션의 비중이 높아지고 있습니다. 그렇다면 모션은 어떻게 적용해야 하는지 알아봅시다.)

![DB 직접수정 스크린샷](/image/그림8.png)

이렇게 설명과 키워드를 넣을 수 있으니, **어떤 내용을** 대해 고민할 때가 됐죠.   
아, 참고로 위 스크린샷은 현재 DB가 아니므로, XSS 하셔도 의미가 없습니다. 그래서 올릴 수 있기도 했고요. 

### 키워드 수집

먼저 저희 비즈니스와 관련된 키워드를 수집합니다. 그 중 가장 기본은 **현재 검색광고 진행중인 키워드**가 되겠죠. 기존 광고 담당자에게 요청하여 검색광고 내역(20개)을 확인합니다. 그리고 그 중 클릭률(CTR)이 가장 높은 키워드(5개)를 선정합니다. 그리고 광고 관리자 내에서 유사 키워드(5000개)를 탐색하고, 그 중 **검색요청 대비 게시글 수가 적은** 키워드(100개)를 엄선합니다. 

> 숫자를 주의해서 봐주세요. 20-5-5000-100 순입니다.   
UX를 분석/제작하는 과정과도 유사하죠?   
기존 경험을 확장하고, 다시 주요 경험으로 집약합니다. 

이렇게 엄선한 키워드는, 저희가 게시물 작성과 키워드 선정, description 등에 사용할 핵심 단어장이 됩니다. 이외의 단어는 매우 중요한 트렌드를 반영하거나, 특별한 목적(설명 목적의 일상용어인 경우 등)이 있어야만 사용 가능하죠. 

keywords와 description 컬럼은 제가 추가했기 때문에, 기존 관리자 페이지에서는 직접 입력이 불가능했습니다. 그나마 다행이라면, SQL 도구가 GUI 기반이었기 때문에 그나마 쉽게 추가할 수 있었죠. 하지만 이렇게 하면 SQL을 사용할 수 없는 경우에는 콘텐츠 작성이 빈약하게 처리된다는 문제가 있었습니다. 

### 관리자페이지 수정

사실, 저 혼자만 처리할 수 있는 일이면 그냥 **메뉴얼 작성**으로 처리하면 됩니다. 그리고 그걸 보면서 **알아서 잘 해보세요** 식으로 떠넘길 수도 있었죠. 그런데, 누군가 drop table 같은 실수를 저지른다는 시나리오가 걱정됐습니다. 무엇보다, **"사용하기 좀 불편하더라도 그냥 견디고 설명서 보세요"** 라고 말하기에는, UX 디자이너로서 자존심이 용납하지 않았어요. 

그래서 수정한 화면을 첨부하려 했는데... admin 페이지라서 이 부분에 대해서는 스크린샷이 없네요. 그냥 간단히 설명하겠습니다. 

- DB와 관련이 없는 페이지(Home, About, List, Contacts)에는 View 쪽에서 직접 키워드/설명 추가
- 관리자페이지에서 글 작성 시 쉼표로 구분하여 입력할 수 있는 입력란 추가, 필수입력 안내
- 한줄요약 입력란 추가, 필수입력 안내
- 키워드/한줄요약 미입력 시 게시물 업로드 불가능하도록 설정
- 모든 게시물은 공통 키워드(Mets HIT)와 카테고리 키워드(Precede, Works, News 등) 자동 입력

> 이외에도 favicon, logo, og:image 등을 설정하는 과정이 있었으나,   
지금까지 설명한 내용과 많이 중복되므로 생략하였습니다. 

이제 진짜로 검색엔진에 크롤링을 요청할 때가 됐습니다. 

## 사이트맵

--------

위 작업까지 끝나고나면, 검색엔진에서는 "[사이트맵](https://www.sitemaps.org/)과 [RSS](https://www.rssboard.org/)를 추가해주세요"라고 말해줍니다. 보통 워드프레스 같은 설치형 블로그를 사용하는경우, 한두가지 플러그인을 적용하여 쉽게 얻을 수 있습니다. 

그런데 사실 RSS는 크게 중요성이 없으며, 최근에는 잘 사용하지 않는 추세이기도 합니다. 게다가 정형화된 콘텐츠 구조가 없는 경우 생각보다 손이 많이 가는 작업입니다. 다만 콘텐츠 자체를 홍보하는 경우, 그리고 RSS를 통한 구독자가 다수 존재하는 경우, 지속적인 유입을 발생시킬 수 있죠. 바로 **인터넷 언론**이 여기에 해당합니다. 저희 비즈니스와는 큰 관계가 없어 이 과정은 생략했습니다. 

> [현재 메츠 홈페이지](https://mets.co.kr)에는 둘 모두 적용돼있습니다   
워드프레스 쓰시고 구원받으세요

하지만 사이트맵은, 검색엔진에서 **그 홈페이지 내 모든 페이지 목록과 실제 검색결과를 비교**하는데 사용하기때문에, 매우 중요도가 높아요. 그나마 다행이라면, 사이트맵 제작은 그리 난이도가 높지 않은 편입니다. 홈페이지 목록과 날짜, 중요도를 입력하면 자동으로 입력해주는 툴이나 웹 기반 서비스가 꽤 많죠. 다만, **우리 서비스의 정보구조(IA)** 에 대해 명확하게 인식하고, 그에 맞추어 사이트맵을 제작해야합니다. 네, 엑셀이 필요한 순간입니다. 

![사이트맵 제작과정](/image/그림9.png)
![사이트맵 예시](/image/그림10.png)

각 항목의 의미는 아래와 같습니다. 
- **loc**   
해당 페이지의 전체 URL. 가능하면 Canonical URL과 동일하게 작성해주시면 좋습니다. 
- **lastmod**   
마지막 수정일. 게시물 발행일과 동일하게 입력하시면 됩니다. 
- **changefreq**   
페이지 갱신 빈도. 목록 링크인 경우 weekly, 홈 화면이나 콘텐츠인 경우 yearly 정도로 입력했습니다. 
- **priority**   
중요도. 0.5~1 사이의 값을 입력하면 됩니다. 홈 화면을 1로 설정하고, 게시물 각각을 0.6으로 설정했습니다. 

이 중 changefreq와 priority는 절대적인 기준이 없으므로, 각 환경에 맞게 정의하시면 되겠습니다.

--------

여기까지 작업을 마치고, 저도 콘텐츠 제작 작업에 참여했습니다. 홈페이지 콘텐츠 중
- [프로토타이핑의 역할 - Mets HIT Inc](https://mets.co.kr/m-lab/ux/why-we-make-prototype/6795/)
- [그래서 인공지능이 대체 뭔가요? - Mets HIT Inc](https://mets.co.kr/m-lab/precede/so-what-is-artificial-intelligence/7631/)

이렇게 두 개는 제가 주도적으로 작업한 게시물이니 한 번쯤 보고오셔도 좋겠습니다. 

-----------

## 결론

2021년 현재, 메츠 홈페이지의 웹표준 순위는 상위 2%입니다. 아래는 방금(2021-03-02) 찍은 스크린샷입니다. 

![현재 웹표준 순위](/image/그림11.png)

이제 게시물을 작성하기만 하면 검색엔진을 통한 유입은 최대한으로 보장됩니다. 그말인즉슨, 작성한 게시물은 어떻게든 검색엔진에 표시되고, SNS로 공유할 경우 항상 요약문과 썸네일이 함께 전송되며, 시각장애인을 위한 접근성 옵션까지 어느정도 충족하고 있다는 뜻이죠. 게다가 모바일이나 태블릿 환경에서 접속하면 그에 맞는 반응형 GUI/UX를 제공할 수 있습니다. 

> 이와 함께 제 [포트폴리오 페이지](https://john33fiao.github.io)를 확인해보니 상위 17%로군요.   
게시물 작성 끝나고 할 일이 생겼습니다. ~~야 신난다~~

사실 저는 이런 **약파는 것 같은 글**을 별로 좋아하지 않습니다. 특히 경영학이나 자기계발서, 처세술 글뭉치에나 등장할만한 글은 더더욱 그렇죠. 특히 "혁신"이라는 말이 등장하는 글은, 개인적인 감상이지만, 별로 가치가 없다고 생각합니다. 

이런 생각이 조금이나마 무뎌지게 된 계기는 바로 [짐 매켈비(2020), &lt;언카피어블&gt;](https://books.google.co.kr/books/about/%EC%96%B8%EC%B9%B4%ED%94%BC%EC%96%B4%EB%B8%94.html?id=nPkIEAAAQBAJ)이라는 책 덕분입니다. 거대한 혁신과 놀라운 아이디어 한두개로 세상이 변한다고 말하지 않아요. 작고 꾸준한 **개선** 수십 수백개가 모여서, 누구도 따라할 수 없는, 아마존이라는 거대 기업조차 빼앗을 수 없는 지분을 차지할 수 있게 된다고 말합니다. 

그리고, 제가 했던 일이 바로 그 **개선**이었음을 알게 되었습니다. 높은 산을 오를 때 자신만이 알고 있는 산꼭대기를 보며 오를 수도 있지만, 보통은 앞을 보며 걷습니다. 그렇게 하나씩 극복하다보면, 어느새 산꼭대기에 있는 자신을 발견할 수 있죠. 그래요, 어차피 정답은 없으니, 지금 당장 할 일을 할 뿐입니다. 

할 수 있고, 해야 한다면, 합니다. 할 수 없는데, 해야 한다면, ~~일단 찡찡대고~~ 배워서 해 볼게요. 

UX 기획, 서요한입니다. 긴 글을 읽어주셔서 감사합니다. 

----------

[홈 화면으로 이동](../)