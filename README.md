### 👻 성장을 이끄는 프레임워크: 프론트엔드 주니어를 위한 네 가지 질문



### 👻 원티드 프리온보딩 챌린지 - CSR / SSR with Next.js

#### 💡 CSR(Client-side Rendering)이란 무엇이며, 그것의 장단점에 대하여 설명해주세요.
   > CSR(Client-side Rendering) : 클라이언트 측에서 페이지를 렌더링하는 방식

   > CSR은 SPA로 동작한다. (SPA(Single-Page Application) : 하나의 페이지로 구성된 웹 어플리케이션)
   > > SPA는 브라우저에서 최초 단 한 번만 페이지 전체(HTML, CSS, JS)를 로드하고 이후 특정 부분만 Ajax를 통해 서버와 데이터를 받아오고 바인딩하는 방식
   > > 즉, 첫 요청시 딱 한번만 페이지만 불러오고 이동 시 기존 페이지의 내부를 수정해서 보여주는 방식이다.
   > > ex) React, Vue, Angular와 같은 자바스크립트 프레임워크들이 SPA의 방식
   >
   > * CSR은 사용자의 요청에 따라 필요한 부분만 응답받아 렌더링 하는 방식이다. 단일페이지(SPA)와 같이 상호작용이 많은 웹 애플리케이션에서 유용하게 사용된다.

* CSR(Client-side Rendering)의 동작방식
  
  (1) 클라이언트가 서버에 페이지를 요청한다. >  (2) 서버는 초기 HTML 및 JS파일을 전송한다.

  (3) 클라이언트가 JS를 실행하여 데이터를 가져와서 동적으로 컨텐츠를 생성한다.  > (4) 생성된 컨텐츠가 화면에 표시된다.



| CSR 장점                                                     | CSR 단점                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **뛰어난 사용자 경험(UX)** : 페이지 로딩 후에도 사용자 상호작용에 대한 빠른 응답이 가능하므로 사용자 경험이 향상된다. | SEO 문제 : 초기 HTML에는 동적으로 생성되는 컨텐츠가 포함되지 않기 떄문에 검색 엔진 최적화(SEO)에 문제가 발생할 수 있다. |
| **서버 부하 감소** : 서버는 초기 페이지를 전송한 후에는 클라이언트에서 대부분의 작업이 이루어지므로 서버 부하가 줄어든다. | 초기 로딩 속도 : 초기 HTML 및 JS파일의 다운로드와 실행에 대한 시간이 필요하므로 초기 로딩 속도가 느릴 수 있다. |
| **캐싱 가능** : 초기 페이지를 제외한 대부분의 자원은 클라이언트에서 동적으로 로드 되므로 캐싱이 용이하다. | 클라이언트 자원 사용량 증가 : 모든 렌더링 작업이 클라이언트에서 이루어지므로 브라우저의 자원(메모리, CPU등)을 더 많이 사용할 수 있다. |


   
 *  SPA(Single Page Application)로 구성된 웹 앱에서 SSR(Server-side Rendering)이 필요한 이유에 대하여 설명해주세요.
   
 * Next.js 프로젝트에서 yarn start(or npm run start) 스크립트를 실행했을 때 실행되는 코드를 Next.js Github 레포지토리에서 찾은 뒤, 
   해당 파일에 대한 간단한 설명을 첨부해주세요.
   
 * https://nextjs.org/docs/getting-started (Next.js 세팅 가이드)
   
 * https://github.com/vercel/next.js/ (Next.js Github 레포지토리)
   
 * _document.js, _app.js, getServerSideProps 같은 요소들에 대해 설명을 요구하는 과제가 아닙니다. 
   오히려 Next.js 코드 베이스 내부를 살펴보라는 의미입니다.
