# 자동차 경주 - TDD

## [1] 문자열 덧셈 계산기 with TDD/Refactoring
### 기능 요구사항
- [x] 기본 구분자 - 쉼표 또는 콜론을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환한다.
    - 예시: “” => 0, "1,2" => 3, "1,2,3" => 6, “1,2:3” => 6
    - [x] 빈 문자열이거나 null 인 경우 0을 반환한다.
  
- [x] 커스텀 구분자 - 문자열 앞부분의 "//"와 "\n" 사이에 위치하는 문자를 커스텀 구분자로 사용한다.
    - 예시: “//;\n1;2;3” -> 커스텀 구분자는 ";", 결과 값으로 6 반환
  
- [x] RuntimeException 예외 던지기
  - [x] 문자열 계산기에 숫자 이외의 값
  - [x] 음수를 전달하는 경우 
<br>
    
## [2] 자동차 경주 게임
### 기능 요구사항
- 자동차 네이밍하기
  - [x] 각 자동차에 이름을 부여할 수 있다.
  - [x] 자동차 이름은 5자를 초과할 수 없다.
  - [x] 자동차 이름은 쉼표(,)를 기준으로 구분한다.

- 자동차 경주 전진 조건
  - [x] 수의 범위는 0 ~ 9 사이의 random 값이다.
    - 수가 음수이거나 9를 초과하면 IllegalArgumentException 예외가 발생한다.
  - [x] random 값이 4이상일 경우 전진한다.
  
- 결과 보여주기
  - [x] 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
  - [x] 게임을 완료한 후 누가 우승했는지 알려준다.
  - [x] 우승자는 한명 이상일 수 있다.
  
### 프로그래밍 요구사항
- 자바 코드 컨벤션 지키기
- indent 는 2까지만 허용
- else 예약어 쓰지 않기
- 3항 연산자 쓰지 않기
- 메소드는 한 가지 일만 하도록 만들기
- UI 로직을 제외한 모든 기능을 TDD 로 구현하기
- 모든 원시 값과 문자열 포장하기
- 일급 컬렉션 쓰기
