# String Calculator

## 요구 사항

### 1. 숫자 합 기능

- 쉼표(,) 또는 콜론(:)을 구분자로 가지는 문자열를 전달할 수 있다.
    - 문자열에 유효하지 않은 값이 있는 경우 경우 예외가 발생한다.(RuntimeException)
        - 숫자 이외의 값(구분자로 등록되지 않은 문자)
        - 음수
- 전달된 문자열을 구분자를 기준으로 숫자들을 분리한다.
- 분리된 숫자들의 합을 반환한다.

```
예)
     "" = 0
  "1,2" = 3
"1,2,3" = 6
"1,2:3" = 6
```

### 2. 커스텀 구분자 기능

- 쉼표(,) 또는 콜론(:) 이외의 커스텀 구분자를 지정할 수 있다.
- 커스텀 구분자는 문자열의 앞부분의 "//" 와 "\n" 사이에 위치하는 문자를 사용한다.

```
예) 커스텀 구분자는 세미콜론(;) 이 지정된다.
"//;\n1;2;3" = 6
```