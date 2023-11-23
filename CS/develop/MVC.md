### MVC 패턴이란?

MVC는 Model, View, Controller의 약자로 프로젝트의 구성요소를 세가지 역할로 구분한 패턴이다.
사용자가 Controller를 조작하면 Controller는 Model을 통해서 데이터를 가져오고, 그 정보를 바탕으로 View를 제어해서 사용자에게 전달하게 된다.

### Model이란?

소프트웨어나 애플리케이션에서 정보 및 데이터 부분을 의미한다. Controller에서 받은 정보를 가공하는 역할을 한다.

#### Model 규칙

사용자가 편집하길 원하는 모든 데이터를 가지고 있어야 한다.

View나 Controller에 대해서 어떤 정보도 알면 안된다.

변경이 생기면 통지에 대한 처리방법을 구현해야 한다.


### View란?

사용자 인터페이스 요소를 나타낸다. 이는 Controller에게 받은 Model의 데이터를 시각적으로 보여주는 역할을 수행한다. 사용자에게 보여지는 화면을 생각하면 된다.

#### View 규칙

Model이 가지고 있는 정보를 따로 저장해서는 안된다.

Model이나 Controller를 알고 있을 필요가 없다.

변경이 생기면 통지에 대한 처리방법을 구현해야 한다.

### Controller란?

Model과 View사이의 데이터 흐름을 제어한다. 사용자가 접근한 URL에 따른 요청을 파악하고 적절한 Method를 호출해 Service에서 비즈니스 로직을 처리한다. 이후 결과를 Model에 저장해 View에게 전달하는 역할을 한다.

#### Controller 규칙

Model이나 View에 대해서 알고 있어야 한다.

Model이나 View의 변경을 모니터링 해야 한다.