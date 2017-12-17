### Concreate class / Abstract class / Trait
+ 어떤 행위를 재사용 하지 않을 경우에는 Concreate class 사용
+ 서로 관련이 없는 클래스들에서 어떤 행위를 여러 번 재사용 해야 할 경우 Trait사용, Trait은 Class Hireachy상의 각기 다른 부분에 삽입 가능
+ Java class에서 Scala class를 상속 받으려면 Abstract class 사용. 단, abstract member만을 가진 Trait은 JVM에서 Java Interface로 변환되므로
그러한 Trait은 Java에서 상속받아 사용할 수 있음. Scala class에서 Java class를 상속 받는 것은 Java class 상속과 동일.
+ Binary형태로 배포하고 외부에서 상속받아서 구현할 때는 Abstract class 사용. 특정 Trait에 memeber를 추가하거나 제가하면 그 Trait를 상속하는 모든 class는 자
자기 자신의 변경 여부에 상관없이 다시 컴파일 해야 함. Trait를 상속하지 않고 호출만 한다면 다시 컴파일 할 필요 없음
+ 성능을 우선시 한다면 Concreate class사용
+ 이러한 경우를 제외하고 재사용이 필요한 대부분의 경우는 Trait 사용, 단, 생성자에 Parameter가 필요한 경우는 Abstact class사용
