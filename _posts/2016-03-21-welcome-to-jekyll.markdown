---
layout: post
title: 무료 다국어 사전 Glosbe API 사용하기
date: 2015-08-27 02:30 +0900
---

## 다국어 사전 Glosbe API

Glosbe는 다국어 온라인 사전이다. 사용자들이 직접 데이터베이스를 보완해 만드는 사전이며 무료다. 아쉽게도 사전의 질은 상용 사전만큼 좋지는 못한 듯하다.

Glosbe는 무료로 웹 API도 제공하기 때문에 다국어 사전이 필요한 경우 이용할 수 있다.

* Glosbe: [https://glosbe.com](https://glosbe.com)
* Glosbe API 페이지: [https://glosbe.com/a-api](https://glosbe.com/a-api)

## Glosbe API 사용하기

Glosbe API 를 사용하려면 다음과 같이 요청을 보내면 된다.

    https://glosbe.com/gapi/translate?from=eng&dest=kor&format=json&pretty=true&phrase=phrase

요청을 보낼 프로토콜과 주소는 `https://glosbe.com/gapi/translate` 이다.

위 예에서 쓰인 매개변수는 다음과 같다.

* `from`: 번역해야 할 단어의 언어 (ISO 693-3 코드)
* `dest`: ~으로 번역되어야 할 언어 (ISO 693-3 코드)
* `format`: 응답 받은 데이터의 유형 (JSON 또는 XML)
* `pretty`: 응답을 사람이 보기 좋게 출력할 것인지 여부 (Boolean)
* `phrase`: 번역해야 할 단어 (대소문자 구분)

