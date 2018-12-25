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
>>> BlockQuote 사용하기4
```
> BlockQuote 사용하기1
> BlockQuote 사용하기2

> BlockQuote 사용하기1
>> BlockQuote 사용하기2
>>> BlockQuote 사용하기3 <br>BlockQuote 사용하기4
>>>> BlockQuote 사용하기4

