# java-racingcar-precourse

# 📝 자동차 경주 기능 목록


## 🔹 사용자로부터 문자열 입력 받기
- 프로그램이 시작되면 사용자가 덧셈할 문자열을 입력할 수 있도록 다음과 같은 문구를 출력한다. `덧셈할 문자열을 입력해 주세요.`
- 사용자로부터 구분자와 양수로 구성된 문자열을 입력 받는다.
- 사용자가 빈 문자열을 입력하면 0 을 반환한다.
  "" => 0
- 그 외에도 형태를 벗어나거나 유효하지 않은 값이 입력되면 예외 처리를 수행한다.


## 🔹 사용자 입력 문자열 분리하기 with 기본 구분자
- 기본 구분자 쉼표(,) 또는 콜론(:)을 기준으로 문자열을 분리하고 숫자 추출

  "1,2:3" => 1 2 3


## 🔹 사용자 입력 문자열 분리하기 with 커스텀 구분자
- 문자열 앞부분 "//"와 "\n" 사이에 커스텀 구분자를 지정한다.

  "//;\n1;2;3" => 1 2 3 (커스텀 구분자: ;)


## 🔹 분리 된 숫자 합산하기
- 구분자를 기준으로 분리된 숫자들을 합산한 후 결과를 출력한다.

  (입력값) 1 2 3 => (결과) 6


## 🔹 입력 값 IllegalArgumentException 예외 처리하기
- 사용자가 잘못된 형식의 문자열을 입력할 경우, 유효하지 않은 값은 예외 처리한다.
- 입력값이 숫자와 구분자가 아닌 경우 모두 예외로 처리
- 단, 공백(빈 문자열)의 경우 예외처리 하지 않고 숫자 0으로 처리

  "1,,2" => 3
- 해당 예외가 발생하면 프로그램을 종료한다.
  


