---
layout: default
title: "JSON을 CSV로 변환하는 방법 | 무료 도구 실습"
description: "DataStudio Lite로 가상의 JSON 데이터를 CSV 표로 바꾸는 초보자용 따라 하기."
lang: ko
date: 2026-11-16
permalink: /ko/guides/json-to-csv/
---

# JSON을 CSV로 변환하는 방법: 무료 도구로 따라 하기

2026년 11월 16일

JSON은 항목마다 이름표가 붙은 형태로 데이터를 담고, CSV는 쉼표로 값을 구분해 표처럼 펼쳐 보여 줍니다. JSON으로 받은 상품 목록을 스프레드시트에서 살펴보고 싶을 때 CSV로 바꾸면 편리합니다. 예제 데이터로 직접 변환해 보겠습니다.

## 준비할 데이터

이번 실습에는 실제 고객 정보가 아닌 가상의 상품 세 건을 사용합니다. 아래 내용을 복사해 둡니다.

```json
[
  {"product": "머그컵", "price": 12000, "stock": 15},
  {"product": "노트", "price": 4500, "stock": 32},
  {"product": "펜 세트", "price": 7800, "stock": 8}
]
```

각 중괄호는 상품 한 건을 나타냅니다. product, price, stock은 CSV에서 열 제목이 됩니다.

## DataStudio Lite에서 변환하기

1. [DataStudio Lite 열기](https://tinkomi.github.io/datastudio-offline-converter/)
2. 화면 위쪽 언어 메뉴에서 한국어를 선택하거나, 영어 화면에서는 **Input Data** 영역을 찾습니다.
3. 입력 영역의 기존 내용을 지우고 위 JSON을 붙여 넣습니다.
4. **JSON → CSV**를 누릅니다.
5. 결과 영역에서 열 제목과 상품 세 건이 제대로 나왔는지 확인합니다.

## 변환 결과

정상적으로 변환되면 다음처럼 표시됩니다.

```csv
product,price,stock
머그컵,12000,15
노트,4500,32
펜 세트,7800,8
```

첫 줄은 열 제목이고 아래 세 줄은 상품 데이터입니다. 예제처럼 입력한 데이터가 세 건이라면 CSV에도 데이터 행이 세 개여야 합니다. 결과 영역에 **Download** 버튼이 표시되며, 확인한 CSV를 파일로 저장할 때 사용할 수 있습니다.

## 결과가 다를 때 확인할 점

- 상품마다 같은 항목 이름을 사용했는지 살펴봅니다. 일부 항목 이름이 다르면 결과 열이 달라질 수 있습니다.
- 쉼표, 따옴표, 대괄호가 빠지지 않았는지 확인합니다. JSON 문법 오류가 있으면 변환이 실패할 수 있습니다.
- 한글이 파일에서 깨져 보이면 파일을 여는 프로그램의 문자 인코딩 설정을 확인합니다.
- 민감한 정보가 든 자료는 실습에 쓰지 마세요. 이번처럼 가상의 값으로 먼저 확인하는 편이 안전합니다.

## 정리

JSON 배열을 입력하고 **JSON → CSV**를 선택하면 표 형태의 결과를 얻을 수 있습니다. 데이터 건수를 비교하고 몇 개 행을 직접 확인하면 변환 과정의 실수를 쉽게 찾을 수 있습니다.

[무료 DataStudio Lite 열기](https://tinkomi.github.io/datastudio-offline-converter/)
