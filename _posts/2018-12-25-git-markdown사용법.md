---
title:  "markdown 사용법"
categories: git
tags: [git, markdown]
toc: true
---

# Markdown 이란?
- 마크다운은 일반 텍스트 문서의 양식을 편집하는 문법이다. README 파일이나 온라인 문서, 혹은 일반 텍스트 편집기로 문서 양식을 편집할 때 쓰인다. 마크다운을 이용해 작된 문서는 쉽게 HTML 등 다른 문서 형태로 변환이 가능하다.

# Markdown 의 장단점

## 장점
1. 간결하다
2. 여러 형태의 변환이 가능하다.
3. 텍스트로 저장되기 때문에 용량 소모가 적다.
4. 지원되는 프로그램과 플랫폼이 다양하다.

## 단점
1. 표준이 없어 사용자에 따라 생성물이 다르다.
2. 모든 HTML 아크업을 대신하진 못한다.

# Markdown 문법

## 제목(header)
`<h1>` 부터 `<h6>` 까지 사용 할 수 있다.
```
# h1
## h2
### h3
#### h4
##### h5
###### h6
```
# h1
## h2
### h3
#### h4
##### h5
###### h6

## 인용문(blockquote)
`<blockquote>` 태그로 변환되어 사용된다.
```
> BlockQuote 사용하기
```
> BlockQuote 사용하기

`<blockquote>` 는 중첩되어 사용할 수 있다.
```
> BlockQuote 사용하기1
> BlockQuote 사용하기2

> BlockQuote 사용하기1
>> BlockQuote 사용하기2
>>> BlockQuote 사용하기3
>>>> BlockQuote 사용하기4
```
> BlockQuote 사용하기1
> BlockQuote 사용하기2

> BlockQuote 사용하기1
>> BlockQuote 사용하기2
>>> BlockQuote 사용하기3
>>>> BlockQuote 사용하기4

## 목록(list)
`<ol>`, `<ul>` 목록 태그로 변환된다.
목록 표시에는 숫자와 기호를 사용하여 표시한다.

- 숫자 목록(번호)
```
1. 첫번째
2. 두번째
3. 세번째
```
1. 첫번째
2. 두번째
3. 세번째

- 기호 목록(기호)
```
- 첫번째
- 두번째
- 세번째

- 첫번째
  - 두번째
    - 세번째

+ 첫번째
+ 두번째
+ 세번째

+ 첫번째
  + 두번째
    + 세번째

* 첫번째
* 두번째
* 세번째

* 첫번째
  * 두번째
    * 세번째
```
- 첫번째
- 두번째
- 세번째

- 첫번째
  - 두번째
    - 세번째

+ 첫번째
+ 두번째
+ 세번째

+ 첫번째
  + 두번째
    + 세번째

* 첫번째
* 두번째
* 세번째

* 첫번째
  * 두번째
    * 세번째

## 강조(emphasis)
`<em>`, `<strong>`, `<del>`, `<u>` 태그로 변환된다.
```
강조는 **별표 2개를 사용** 하거나 __언더바 2개를 사용__ 한다.
이텔릭 글씨는 *별표 1개를 사용* 하거나 _언더바 1개를 사용_ 한다.
취소선은 ~~물결 표시를 사용~~ 한다.
밑줄은 <u>밑줄</u>을 사용 한다.
```
강조는 **별표 2개를 사용** 하거나 __언더바 2개를 사용__ 한다.<br>
이텔릭 글씨는 *별표 1개를 사용* 하거나 _언더바 1개를 사용_ 한다.<br>
취소선은 ~~물결 표시를 사용~~ 한다.<br>
밑줄은 <u>밑줄</u>을 사용 한다.

## 코드(code)
`<pre>`, `<code>` 로 변환된다.
입력 방법은 ` (Grave)를 사용하여 입력한다.

### 인라인(inline) 코드
```
인라인 코드는 `사용하고 싶은 문장에 Grave를 붙여` 사용한다.
```
인라인 코드는 `사용하고 싶은 문장에 Grave를 붙여` 사용한다.

### 블록(block) 코드
```
블록 코드는 Grave를 세번이상 입력해야 한다.
```

## 링크(link)
링크는 `<a href="">` 처럼 사용된다.
링크에는 인라인 링크, 참조링크, 자동연결이 있다.
```
- 인라인링크
[구글](https://google.com)
[naver](https://naver.com "네이버로 이동하기")

- 참조링크
[구글로가기][google]
[github][깃허브]
참조링크는 [참조링크]바로 사용할 수 있다.
[상대적참조](../tags/git)

[google]: https://google.com
[깃허브]: https://github.com
[참조링크]: https://google.com

- 자동연결
https://google.com
<https://google.com>
```
- 인라인링크<br>
[구글](https://google.com)<br>
[naver](https://naver.com "네이버로 이동하기")

- 참조링크<br>
[구글로가기][google]<br>
[github][깃허브]<br>
참조링크는 [참조링크]바로 사용할 수 있다.<br>
[상대적참조](../tags/git)

[google]: https://google.com
[깃허브]: https://github.com
[참조링크]: https://google.com

- 자동연결<br>
https://google.com<br>
<https://google.com>

## 수평선(horizontal Rules)
수평선은 `<hr>` 처럼 사용된다.
`-`, `*`, `_` 중 선택하여 3개 이상을 작성하면 된다.
```
---
***
___
-----------------
```
---
***
___
-----------------

## 이미지(image)
이미지는 `<img>` 처럼 사용된다.
이미지에는 인라인이미지, 링크이미지, 참조이미지가 있다.
```
- 인라인이미지
![gitLogo](/asset/images/gitlogo.png)

- 링크이미지
![googleLogo](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png)

- 참조이미지
![gitLogo][1]
[1]:/asset/images/gitlogo.png
```
- 인라인이미지<br>
![gitLogo](/assets/images/gitlogo.png)

- 링크이미지<br>
![googleLogo](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png)

- 참조이미지<br>
![gitLogo][1]
---
[1]:/assets/images/gitlogo.png
