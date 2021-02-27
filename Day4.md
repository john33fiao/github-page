# SEO 진행과정

[홈페이지 마케팅](#) 에서 이어지는 글입니다. 

과정이 생각보다 길어서 다른 글로 분리해서 이야기해보려 합니다. SEO 작업을 진행한 URL은, 현재 새로운 콘텐츠로 완전히 변경하였습니다. 그리고 기존 코드와 콘텐츠는 모두 회사 내부 서버에만 존재하죠. 그래서 이 과정을 공개할 수 있었습니다. 

이렇게 진행한 과정은, 사실, [메츠에이치아이티 홈페이지](https://mets.co.kr)라는 조건에서 진행한 이야기라서, 공통 가이드가 되기는 어려울지도 모르겠습니다. 

혹시 저 링크를 눌러보셨으면 아시겠지만(눌러주세요, 나름 열심히 구축했어요), GUI/UX 전문회사입니다. 즉, 디자이너만 많고, 그 중 기획(겸 개발)자 하나 있었죠. 당시 사용중이던 홈페이지는 제가 입사하기 2년 정도 전에 구축이 완료됐고, 웹개발 업체에 외주를 맡겨서 진행했다고 합니다. 그런데 해당 업체에서는 내부 솔루션을 그대로 적용하였기에, 보안은커녕 콘텐츠 갱신조차 제대로 이루어지기 어려운 상황이었습니다. ~~사실, 이 때 SEO 작업을 포기해야 했습니다.~~ 그런 의미에서, 저는 진심어린 조언을 남겨둡니다. 

> 어지간하면, 할 줄 안다고 말하지 마시고요,   
조용히 맨먼스 산정해서 견적서 제출하세요.

아래 **나열** 한 과정은 개발에 대한 기본 지식이 있으시다면 쉽게 따라할 수 있습니다. [생활코딩 WEBn](https://opentutorials.org/course/3083)과정을 공부하셨다면, 저보다 더 나은 방법으로, 더 좋은 결과물을 만드실 수도 있습니다. 그런데 만약 개발에 대해 문외한이시고, 크롬 DevTools 조차 써본 적 없으시다면... 바로 위에 적어둔 **진심어린 조언** 을 기억해주세요. 각 홈페이지 환경, 심지어 개별 조직 환경에 따라서도 전혀 불가능할 수 있기 때문입니다. 

그리고 이 과정을 시작하기 전, 한 가지 기억해주셔야 할 문구가 있습니다. 

## Don't be Evil

정작 구글에서는 이제 사용하지 않는 문구니까 저는 자유롭게 사용하겠습니다...라고 쓰려다가 확인해보니 아직 남아있네요. 심지어 더 좋은 문구로 바뀌었습니다. 2020-09-25에 업데이트된 [구글 행동강령](https://abc.xyz/investor/other/google-code-of-conduct/)에서 **VIII. Conclusion** 부분을 확인해보세요. 

이 정신을 따라서, 저도 옳은 방법만을 사용했습니다. 연관키워드를 탐색하기 위해 크롤링을 돌리거나, 유입을 강제로 늘리기 위해 조회수를 구입할 수도 있었습니다. 심지어 타사 홈페이지나 블로그 등에 스팸 댓글을 남겨서 어떻게든 핑백을 올리는 방법도 있었습니다. 하지만, 그러지 않는 편이 장기적으로 더 낫다고 생각했습니다. 무엇보다, 저 스스로가 이 과정을 진지하게 배워보고자 했습니다. 결국 꽤 힘든 길이 됐지만 말이죠. 

**비극은 멀리서 보면 희극이라 하였습니다.** 다행히 이제 꽤 지난 일이라 즐겁게 이야기할 수 있네요. 그럼 지금의 저와 함께, 멀리서 희극으로 바라봅시다. 이제, 시작합니다. 

## 상태 점검

지피지기면 백전불태라 하였습니다. 무언가 개선이 필요하다고 인식하려면, 먼저 현재 상태를 점검해야겠죠. 당시 저는 회사 홈페이지에 들어가본 뒤 *"깔끔하고 예쁘게 잘 만들었네. 콘텐츠 수가 좀 적기는 하지만, GUI/UX 포트폴리오를 보여주기는 충분하지 않나?"* 라고 쉽게 생각했습니다. 하지만 그게 아니었죠. 

[DevTool](https://developers.google.com/web/tools/chrome-devtools) 콘솔을 열고, 클릭 영역을 확인합니다. 해상도 반응형 UX가 적용됐음을 확인하고, 가끔 오류가 날 때도 있기는 하지만 그래도 새로고침을 하면 문제 없이 표시됨을 보며 좋아했습니다. 그래요, 별로 할 일이 없어보였죠. 그래서, 얼마나 많은 사람들이 저희 콘텐츠를 보러 오는지 확인하고 싶었습니다. 

### 트래픽 조회

먼저, 홈페이지 유입 트래픽을 조회하기 위해 호스팅사 관리자페이지를 확인했습니다. 그런데 예상보다 트래픽 용량을 엄청나게 많이 사용하고 있었습니다. 그래서 저는 *"뭐야 생각보다 인기 많은 곳이었나?"* 싶었죠. 그래서 유입 IP를 확인하니... 스팸 IP가 대부분이었습니다. 일단 해당 IP 및 주요 스팸 유입국가에 대해 진입 차단을 걸었죠. 

국가단위 차단을 해도 괜찮을까 조금 고민했는데, 답은 의외로 가까운 곳에 있었습니다. 바로, 키워드 광고 집행비용 대비 유입이었죠. 메츠는 네이버 검색광고를 항상 집행하고 있습니다. 그런데 키워드 광고비 집행비용에 비해 유입이 지나치게 많았고, 무엇보다 메츠는 폴란드, 스웨덴, 슬로바키아 업체로부터 GUI/UX 제작 의뢰를 받을 일이 별로 없었습니다. 

### 콘텐츠 조회

다음으로 홈페이지 콘텐츠를 점검했습니다. 마지막 업로드 콘텐츠가 2017년인 사실은 둘째치고, 모든 게시글에 스팸 댓글이 달려있었습니다. 사실, 이 댓글 내용도 좀 진지하게 읽어보려했는데, 알고보니 Lorem Ipsum 수준으로 아무 키워드나 적어두고 특정 서비스 하이퍼링크를 달아 둔 형태였습니다. 그래서 일괄 삭제를 위해 홈페이지 admin 페이지 아이디와 암호를 요청했습니다. 

그리고 저는 이전 기획자가 남겨둔 인수인계 문서를 확인했습니다. 관리자페이지 로그인 ID는 admin, 비밀번호는 1234였습니다. 당황 겸 분노해서 일단 로그인을 했죠. 그리고 급하게 그 비밀번호를, 회사 내 표준 비밀번호 형식에 맞추어 수정 후 공유했습니다. 

그 다음에는 스팸댓글 일괄 삭제를 위해 홈페이지 관리자페이지를 들어갔는데... 댓글 관리 기능이 없었습니다. 저는 그 즉시, 기존 홈페이지를 구축한 업체에 연락하고 하루를 기다렸습니다. ~~그리고 2년이 넘게 지난 지금도 아직 답은 오지 않음~~  

사실, 이 때까지만 해도 포기할 수 있었습니다. 그런데 당시에는 연말이라 큰 프로젝트가 없다시피했고, 당시 저는 애사심이 꽤 많이 남아있던 상태였습니다. ~~신성한 홈페이지에 어딜 감히 스팸이야!~~ 댓글 일괄 삭제를 위해, 데이터베이스 직접 접근을 시도합니다. 

## SQL

보통 웹페이지에 표시되는 콘텐츠는 HTML 형식으로 데이터베이스(Database, DB)에 보관됩니다. 개별 웹페이지를 하나하나 저장하면 용량을 매우 많이 차지하기도 하고, 무엇보다 관리가 힘들기 때문이죠. 그리고 이 DB는, [SQL](https://ko.wikipedia.org/wiki/SQL)을 사용하여 접근합니다. 그런데 DB 접근을 위해서는, DB 전용 계정과 비밀번호가 필요하죠. 그래서 호스팅사에 DB 계정 정보를 요청하고, 하는 김에 FTP 접근 권한도 요청했습니다. 그리고, 호스팅사 [WAS(웹 애플리케이션 서버)](https://ko.m.wikipedia.org/wiki/%EC%9B%B9_%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98_%EC%84%9C%EB%B2%84) 내에 [phpMyAdmin](https://www.phpmyadmin.net/)을 설치했습니다. 불행인지 다행인지, 댓글 DB에는 스팸밖에 없어서 모두 삭제해도 큰 문제가 없었습니다. 

이렇게 기존 스팸댓글은 삭제했지만, 이걸 그대로 두면 앞으로도 스팸 댓글이 쌓일 것 같았죠. 그래서, 아예 소스코드를 열어 댓글 영역을 가림처리(display:none) 하였습니다. 

이 과정에서 콘솔을 다시 열어보니, JavaScript 오류가 넘쳐나고 있었죠. 차근차근 읽어보니, 개발사에서 페이스북 댓글 기능을 연동하기 위해 설치한 페이스북 픽셀이, 현재 사용중인 [메츠 페이스북 페이지](https://www.facebook.com/metshit)와 연동되지 않은 문제가 있었습니다. 위에서 언급했다시피, 기존 개발사로부터의 개발 문서는 아직 수령하지 못한 상태였습니다. 

어차피 사용하지 않는 댓글 영역이었고, 무엇보다, 회사 홈페이지라는 조건에서 댓글 영역은 장점보다 단점이 더 많다는 판단 하에, 댓글 뷰 영역을 주석처리 했습니다. 

> 사실, 소스코드 내에 주석을 몇 글자 더 적었습니다.  // 도망쳐

이 때도 저도 도망칠 기회가 있었습니다. 하지만 이 부분도 이미 말했다시피, 연말이라 일이 별로 없었어요. 홈페이지 관리를 제대로 해보기로 했으니, 홈페이지 내에 방문자 추적 툴을 설치합니다. 

### 애널리틱스

일반적으로, 대부분의 웹페이지에는 방문자 추적 툴이 설치돼있습니다. ~~물론 저희 홈페이지에는 없었고요~~ 방문자가 주로 유입되는 검색엔진(구글, 네이버, 다음,  Bing, Yandexy 등)이나, 유입 경로(카카오톡, 페이스북, 핀터레스트 등)를 확인하기 위해서죠. 이러한 도구는 보통 무료로 제공되는 경우가 많습니다. 하지만 유료 서비스를 이용하면 대규모 서비스나 상세 통계, 심지어 마우스 클릭 위치 등을 확인할 수도 있습니다.


애널리틱스를 제공하는 기업은 다음과 같습니다. 

- [구글 애널리틱스](https://analytics.google.com)   
유/무료 모두 있습니다. 일반적인 용도에서는 무료 서비스만으로 충분합니다. 데이터 표시형식을 커스텀 할 수 있어, SEO 작업을 진행하기 전 필수로 설치합니다. 대규모 서비스에 적용하는 경우 유료 서비스인 [GA360](https://marketingplatform.google.com/intl/ko/about/analytics-360/)을 사용하는 방법도 있습니다.   
- [네이버 애널리틱스](https://analytics.naver.com)   
무료 서비스입니다. 일반적으로 사용하기에는 충분한 데이터를 제공합니다. 네이버에서 제공하는 툴이므로, 네이버로부터 유입되는 데이터를 정말 잘 분류해줍니다. 국내 시장을 기반으로 하는 상품/서비스인 경우 반드시 설치해야합니다.    
- [뷰저블](https://www.beusable.net/)   
1주일 무료체험 후 유료로 전환됩니다. 마우스 위치에서부터 클릭 위치, 스크롤 수준, 각 페이지별 잔류시간 등, **사용성 테스트**에서나 얻을 수 있는 소중한 데이터를 제공합니다. 무료 사용이라도 한 쯤 이용해보심을 추천합니다. 
- [Adobe 애널리틱스](https://www.adobe.com/kr/analytics/adobe-analytics.html)   
유료로 제공하는 애널리틱스 툴이며, 대규모 서비스에 주로 적용합니다. 각 채널별 데이터에서부터 고객 생애 가치까지, 다양한 정보를 제공합니다. 또한 대부분의 기능을 직접 설정해야하는 GA와는 달리, 사용성 측면에서 큰 강점이 있다고 합니다. 

애널리틱스는 웹페이지 내에서 JavaScript 기반으로 작동하므로, 웹페이지 소스코드를 직접 수정해야합니다.

모든 페이지에서 공통으로 사용하는 태그 부분에 애널리틱스 코드를 추가하면 되는데요, 보통 Header나 Footer 파일에 추가합니다. 각 애널리틱스에서 공식적으로 권장하는 방법은 </body> 바로 앞에 추가하는 방법으로, 일반적으로는 Footer에 해당합니다. 이렇게 하면 웹페이지 진입 후 로딩이 완료된 시점에 방문을 기록하게 됩니다. 

이 시점에서 한 가지를 확인해야 하는데요, 자사 홈페이지 주소가 http로 시작하는지, https로 시작하는지입니다. https 웹페이지는 크로미움 기반 웹브라우저에서 볼 경우 주소표시줄 앞에 자물쇠 그림이 표시됩니다. 즉, SSL 인증서를 통한 웹페이지 보안을 적용중이라는 뜻이지요. 기본적으로 애널리틱스는 방문자의 개인정보를 기록하는 과정이기때문에, 최소한이라도 개인정보 보호 조치가 필요합니다. 그리고 그 중 첫 번째 단계가 바로 SSL입니다. 

### HTTPS(HTTP over SSL)

[HTTPS](https://ko.wikipedia.org/wiki/HTTPS)는 개인정보 보호 차원에서도 중요하지만, 중복 URL을 제거할 수 있어 검색엔진 최적화에 영향을 줍니다. 게다가 구글에서는 SSL 인증서가 있는 경우 [검색 결과에 더 많이 표시](https://developers.google.com/search/blog/2014/08/https-as-ranking-signal)하겠다고 발표한 바 있습니다. 저야 그냥 혹시나 몰라서(개인정보 보호법 무서워요) 설정했고, SEO에 영향을 준다는 사실은 훨씬 나중에 알았습니다. 

호스팅사를 통해 Codomo에서 SSL 인증서를 구입하고, 호스팅사 관리자페이지에서 SSL을 등록합니다. 하지만, 여기서 끝날 수 있었으면 참 행복했겠지요. 아무리 해도 자동으로 SSL 적용된 화면으로 이동하지 않았습니다. 심지어 인증서가 잘 작동하지 않는 것처럼 보여서, 오히려 보안에 취약한 페이지처럼 보이기도 했죠. 결국 [MVC 설계](https://developer.mozilla.org/ko/docs/Glossary/MVC) 중 컨트롤러(Controller) 부분을 수정하게됩니다. 

그런데 마저 이야기하기 전에, 잠시 쉬어가겠습니다. 다음 글에서 만나요. ~~도망치라니까요~~