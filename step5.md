## 리팩토링 요구사항
- 핵심 비지니스 로직을 가지는 객체를 domain 패키지, UI 관련한 객체를 view 패키지에 구현한다.
- **MVC 패턴 기반으로 리팩토링해 view 패키지의 객체가 domain 패키지 객체에 의존할 수 있지만, domain 패키지의 객체는 view 패키지 객체에 의존하지 않도록 구현**한다.

## 리팩토링 대상 선정
- [X] CarStatus를 제거하고 ResultView로 출력 로직을 좀 더 위임 등의 방향
- [X] Cars의 기본 생성자의 접근 제어가 변경 및 정적 팩토리 생성자 활용하기
- [X] View는 Domain 패키지에 의존할 수 있지만, Domain은 View를 의존하지 않는 구조로 변경
