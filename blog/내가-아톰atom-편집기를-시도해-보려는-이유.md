# [내가 아톰(Atom) 편집기를 시도해 보려는 이유](https://only2sea.wordpress.com/2016/02/10/내가-아톰atom-편집기를-시도해-보려는-이유/) #

[고(Go)](https://golang.org) 언어 책을 쓰느라 [아톰 편집기](https://atom.io/)를
잠시 사용해 본 적이 있는데, 필요한 부분만 확인하고 더 사용하지 않았다. 주력
편집기(서식 없는 글을 주로 편집하는 컴퓨터 소프트웨어)로
[이맥스(Emacs)](https://www.gnu.org/software/emacs/)를 쓰고 있는데 시대에 조금
뒤떨어진 부분도 있지만 마음대로 커스터마이즈 하기 어려운 편집기를 쓰고 싶지
않아서 계속 쓰고 있었다.

사실 이맥스는 편집기라기보다는 리습(LISP)코드들을 돌리는 인터프리터이며 일관된
인터페이스였다. 이 인터페이스가 편리해서 이맥스를 쓰는 것이다. 동일한 단축키와
사용법을 유지할 수 있다. 문서를 작성할 때, 프로그램 코드를 작성할 때, 이메일을
작성할 때, 쉘에서 명령을 내릴 때, 심지어는 음악을 들을 때에도 서로 다른 단축키와
인터페이스를 이용하는 것보다는 동일한 인터페이스를 이용하는 것이 편리하다.

이런 환경이 어디에 있을까 고민하던 중에 웹 브라우저가 사실상 이맥스와 비슷하다는
생각을 했다. 웹 브라우저는 자바스크립트라는 언어의 인터프리터이며 이것이 DOM을
제어하게 하여 일관된 인터페이스를 제공할 수 있는 것이었다. 자바스크립트 코딩은
놀랄만큼 리습 코딩과 비슷하며, 웹 앱의 거의 모든 기능을 스크립트로 제어할 수
있다. 웹 브라우저를 이맥스와 비교했을 때 좋은 점과 나쁜 점이 있다.

**좋은 점:**

  * 글자 단위의 개념에 갖혀 있지 않아서 훨씬 자유로운 레이아웃과 스타일, 이미지
    등의 기능을 제공한다. 이맥스에서는 동영상을 내장하거나 복잡한 CSS로 표현을 할
    수 없기 때문에 여러가지로 UI가 제한된다.
  * 이맥스보다 사용자 층이 훨씬 넓고 훨씬 더 많은 현대적인 애플리케이션들이
    있다.

**나쁜 점:**

  * 중요한 단축키들을 브라우저가 다 잡아먹고 있어서 웹앱들이 이것을 이용하기
    어렵다.
  * 키보드 친화적인 인터페이스가 구축이 잘 되어 있지 않아서 불편한 점이 많다.

브라우저와 이맥스의 단축키를 생각해 보자.

  * `Ctrl+S`가 브라우저에서는 저장 단축키지만 이맥스에서는 찾기 기능이 `Ctrl+S`에
    기본으로 할당되어 있다. 이맥스에서 저장을 하려면 `Ctrl+X S` 단축키를 눌러야
    한다.
  * 이맥스에서 `Ctrl+T`는 커서 위치의 문자의 위치를 바꾸는 단축키이지만,
    브라우저에서는 새 탭을 여는 단축키이다.

많은 예를 들지는 않았지만 당연하게도 브라우저에서는 웹 브라우징을 하는데 중요한
단축키들이 배치되어 있고, 이맥스에서는 텍스트를 편집하는데 중요한 단축키들이
배치되어 있고, 그렇지 않은 키들은 더 복잡한 단축키로 구성되어 있다. 브라우저에서
텍스트를 편집하기 위한 단축키는 `Ctrl+Z,X,C,V,A` 정도다.

따라서 브라우저의 렌더링 엔진과 자바스크립트 인터프리터는 그대로 두되, 단축키는
텍스트 편집을 위한 것들을 편리하게 배치하고 브라우징을 위한 단축키들은 좀
불편하게 배치하면 어떨까? 그렇게 하기만 해도 웹에서 텍스트를 편집하는 것을 주요
업무로 삼을 때는 더 편리한 브라우저가 나올 것 같았다.

물론 편집기의 단축키들을 이용할 수 있게 해 주는 브라우저 확장들을 사용해 보기는
했지만, 이 확장들은 결국 자바스크립트로 돌아가는 것이라 브라우저 바이너리가 미리
선점해 놓은 것들은 어쩔 수 없었다. 예를 들어서 `Ctrl+N`을 누르면 항상 새 창이
뜬다.

아마 아톰 편집기가 나 같은 필요성을 느끼는 사용자들을 겨냥한 것이라
생각한다. 그래서 아톰을 써 보려고 한다. 일단 첫 인상은 여러가지 답답함이
있다. 생각보다 유연하지 않을 수도 있는데, 일단은 좀 배워보려고 한다.

이맥스를 쓰던 사용자라면 편집기 안에서 모든 일을 하고자 할 것이다. 이맥스 안에서
웹 브라우징도 할 수 있다. 장점은 편집기의 인터페이스를 이용해서 웹 페이지를
돌아다니고 복사하고 붙이고 문서에 있는 코드를 바로 실행해 볼 수 있다. 아톰에도
브라우저 플러그인이 있는데 그렇게 구현되지는 않은 듯 하다. 좋은 점은 아마도 크롬
인스턴스를 2개 띄울 필요가 없어서 리소스를 좀 아낄 수 있다는 것 정도일까?

10년 쯤 전에 주력 편집기를 빔(Vim)에서 이맥스로 넘어왔는데 아톰으로 넘어가려는
시도는 성공할지, 실패할지, 아니면 별로 좋지 않아서 다시 돌아올지 아직은 잘
모르겠다.
