# 115. 정수 데이터의 비트 패턴 출력하기

**난이도:** ★☆☆☆☆

## 문제

0 이상 255 이하의 정수를 입력받아 8비트 2진수 패턴(앞자리 0 포함)으로 출력하세요.

[입력] 정수 (0~255)
[출력]
(8자리 2진수)

## 내 코드

```c
#include <stdio.h>

int main(void) {

    int n;
    scanf("%d", &n);
    for (int i = 7; i >= 0; i--)
        printf("%d", (n >> i) & 1);
    printf("\n");
    return 0;
}

   
```

## 모범 답안

```c
#include <stdio.h>
int main(void)
{
    int n;
    scanf("%d", &n);
    for (int i = 7; i >= 0; i--)
        printf("%d", (n >> i) & 1);
    printf("\n");
    return 0;
}
```

_해결일: 2026-11-24_