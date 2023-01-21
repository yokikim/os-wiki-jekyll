---

layout: post

---

70p

응용 프로그래밍 인터페이스 Application Programming Interface

간단한 프로그램이라도 운영체제의 기능을 아주 많이 사용하게 된다.

종종 초당 수천 개의 [[시스템 콜]]을 수행하게 된다.

사용자 대부분은, 이러한 정도의 상세를 결코 알지 못한다.

대부분의 응용 개발자들은 응용 프로그래밍 인터페이스에 따라 프로그램을 설계한다.

API는 각 함수에 전달되어야 할 매개변수들과 프로그래머가 기대할 수 있는 반환 값을 포함하여 응용 프로그래머가 사용 가능한 함수의 집합을 명시한다.

프로그래머는 운영체제가 제공하는 코드의 라이브러리를 통하여 API를 활용한다.

UNIX 와 Linux 시스템에서 C 언어로 작성된 프로그램을 위해서 제공되는 라이브러리는 libc로 불린다.

막후에서 API를 구성하는 함수들은 통상 응용 프로그래머를 대신하여 실제 시스템 콜을 호출한다.

왜 응용 프로그래머는 실제 시스템 콜을 부르는 것보다 API에 따라 프로그래밍 하는 것을 선호하는가? 그렇게 하는 데에는 몇 가지 이유가 있다.

한 가지 이점은 프로그램의 호환성과 관련 있다.

API에 따라 프로그램을 설계하는 응용 프로그래머는 자신의 프로그램이 같은 API를 지원하는 어느 시스템에서건 컴파일되고 실행된다는 것을 기대할 수 있다.

(현실적으로는 컴퓨터 구조의 차이 때문에 보이는 것보다 쉽지는 않다.)

게다가 실제 시스템 콜은 종종 좀 더 자세한 명세가 필요하고 프로그램상에서 작업하기가 응용 프로그래머에게 가용한 API보다 더 어렵다.

그럼에도 불구하고 API 함수를 호출하는 것과 커널의 관련된 시스템 콜을 호출하는 것에는 강한 상관관계가 존재한다.

---

[[실행시간 환경]] (RTE)

[[시스템 콜 인터페이스]]