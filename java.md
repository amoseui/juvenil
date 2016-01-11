
##Head First Java
---

7. 상속과 다형성

	- 하위클래스와 상위클래스 사이에서 'A는 B다' 관계가 성립하지 않는다면 상속을 사용하면 안 된다.



8. 인터페이스와 다형성

	- 컴파일러에서는 추상 클래스의 인스턴스를 만드는 것을 허용하지 않는다.

	- 추상 클래스: 반드시 확장해야하는 클래스

	- 추상 메소드: 반드시 오버라이드해야하는 메소드

	- 추상 클래스가 아닌 클래스에 추상 메소드를 집어넣을 수는 없다.

	- 컴파일러에서 어떤 메소드를 호출할 수 있는지 결정할 때는 실제 객체 유형이 아닌 레퍼런스 유형을 기준으로 따진다.

	- 레퍼런스 변수의 클래스에 들어있는 메소드를 사용한다.

	- 인터페이스 메소드는 자동으로 public, abstract가 된다. (생략 가능)



9. 생성자와 가비지 컬렉션

	- 지역 변수가 객체에 대한 레퍼런스인 경우에는 변수만 스택에 들어간다. 객체는 여전히 힙 안에 있다.

	- 생성자의 가장 중용한 특징은 객체가 레퍼런스에 대입되기 전에 실행된다는 점이다.

	- 생성자에서 super()를 호출하지 않으면 컴파일러가 알아서 상위 클래스의 인자가 없는 생성자를 호출한다.

	- super()를 호출하는 선언문은 모든 생성자의 첫번째 선언문이어야 한다.

	- 모든 생성자에는 super() 또는 this()를 호출하는 선언문이 들어갈 수 있지만 둘 다 쓸 수는 없다.

	- 객체의 레퍼런스를 제거하는 세 가지 방법

		- 레퍼런스가 영원히 영역을 벗어난다.

		- 레퍼런스에 다른 객체를 대입한다.

		- 레퍼런스를 직접 null로 설정한다. 