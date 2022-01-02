## BeanFactory와 ApplicationContext

### BeanFactory

    - 스프링 컨테이너의 최상위 인터페이스이다.

    - 스프링 빈을 관리하고 조회하는 역할을 담당한다.

    - getBean() 을 제공한다.

    - 지금까지 우리가 사용했던 대부분의 기능은 BeanFactory가 제공하는 기능이다.

### ApplicationContext

    - BeanFactory 기능을 모두 상속받아서 제공한다.

    - 빈을 관리하고 검색하는 기능을 BeanFactory 가 제공해주는데, 그러면 둘의 차이가 뭘까?

    - 애플리케이션을 개발할 때는 빈은 관리하고 조회하는 기능은 물론이고, 수 많은 부가기능이 필요하다.

### 정리

    - ApplicationContext는 BeanFactory의 기능을 상속받는다.

    - ApplicationContext는 빈 관리기능 + 편리한 부가 기능을 제공한다.

    - BeanFactory를 직접 사용할 일은 거의 없다. 부가기능이 포함된 ApplicationContxt를 사용한다.

    - BeanFactory나 ApplicationContext를 스프링 컨테이너라 한다.