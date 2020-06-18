---
title: "[프로그래머스/javascript] 1. 자릿수 더하기"
date: 2020-06-17 08:26:28 -0400

categories:
  - Study
tags:
  - 프로그래머스
  - javascript
---

## 문제 설명

자연수 N이 주어지면, N의 각 자릿수의 합을 구해서 return 하는 solution 함수를 만들어 주세요.
예를들어 N = 123이면 1 + 2 + 3 = 6을 return 하면 됩니다.

제한사항
N의 범위 : 100,000,000 이하의

## 문제 풀이

```
function solution(n)
{
    var answer = 0;
    var number = String(n);

    for(var i=0; i<number.length; i++){
        answer+=parseInt(number[i])
    }
    // [실행] 버튼을 누르면 출력 값을 볼 수 있습니다.
    console.log('Hello Javascript')

    return answer;
}
```

## POINT

#### parseInt()

- 문자열 인자의 구문을 분석해 특정 진수(수의 진법 체계에 기준이 되는 값)의 정수를 반환합니다.

- 구문

```
parseInt(string, radix);
```

**string**
분석할 값. 만약 string이 문자열이 아니면 문자열로 변환(ToString 추상 연산을 사용)합니다. 문자열의 선행 공백은 무시합니다.

**radix**
string이 표현하는 정수를 나타내는 2와 36 사이의 진수(수의 진법 체계에 기준이 되는 값).

[참고사이트](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/parseInt)
