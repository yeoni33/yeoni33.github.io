---
layout: post
title: "JavaScript"
date: 2022-01-06
excerpt: "JavaScript란?"
categories: javaScript
tags: [study, JavaScript]
comments: true
---

<style>
	h3{
		background-color:#D2D2FF;
		color: gray;
	}
</style>

<h3>1. JavaScript</h3>

 - 웹에서 가장 많이 쓰이는 `인터프리터방식` 스크립트 언어로 웹의 동작을 구현한다.
 - 역할
	- HTML 페이지 변경 및 엘리먼트 추가, 제거
	- CSS와 HTML 엘리먼트의 스타일 변경
	- 마수스나 키보드 이벤트에 대한 스크립트 실행
	- AJAX를 이용한 웹 서버 통신
	- 기타 동적 효과 등등
 - 자바와 비교
 <table>
	<tr align="center">
		<th>JavaScript</th>
		<th>Java</th>
	</tr>
	<tr align="center">
		<td>OOP 스크립팅 언어</td>
		<td>OOP 프로그래밍 언어</td>
	</tr>
	<tr align="center">
		<td>코드가 모두 텍스트</td>
		<td>컴파일 필요</td>
	</tr>
	<tr align="center">
		<td>HTML과 CSS가 있어야 실행(의존적)</td>
		<td>다양한 OS에서 실행 가능한 독립적인 언어</td>
	</tr>
	<tr align="center">
		<td>자료형 선언 불필요</td>
		<td>자료형 선언 필수</td>
	</tr>
	<tr align="center">
		<td>생성자 정의 필요</td>
		<td>생성자 정의 불필요</td>
	</tr>
</table>
<br>

<h3>2. 장단점</h3>

 - 장점 : 컴파일을 하지 않아 속도가 빠르고 구조가 단순하여 배우기 쉬움. 웹에 특화된 기술이므로 종속성이 낮고 확장성 높음
 - 단점 : 개발도구가 적고 기능이 제한적임. html 소스코드에 같이 작성시 코드가 노출되어 보안에 취약함
<br>


<h3>3. 사용법</h3>

 1. inline(인라인) : 태그 내에 간단 소스코드를 작성해서 실행
	`<태그 on이벤트명="해당요소에 해당이벤트 발생시 실행할 소스코드 | 함수명();">`
 2. internal(내부) : html 문서내에(head, body 상관없음) script 태그 기술하여 그 영역안에 소스코드를 작성
 3. external(외부) : 별도의 .js 파일로 소스코드를 작성하고 html문서 내에 `<script src="경로">` 표기 후 사용

<br>


<h3>4. Window, DOM, BOM이란</h3>

 1. window 객체
	- 자바스크립트의 최상위객체이자 전역객체로 크게 DOM과 BOM으로 나뉨
	- 개발자 도구에서 window우 출력 시 window객체를 이루는 구성 요소들을 볼 수 있는데 자바스크립트는 이 객체들을 제어함으로써 웹 브라우저를 제어하는 것 
	<figure>
	<img src="https://user-images.githubusercontent.com/93863500/148331222-63bdab9f-b7cf-4ec8-a22a-452cbee01560.JPG" width="100%" height="100%" align="center">
	</figure>
<br>
 
 2. DOM(Document Object Model)
	- 브라우저가 웹문서를 이해할 수 있도록 요소들의 관계를 트리 구조로 구성한 것
	- HTML의 각 요소들을 노드(Node)라고 하며 주로 쓰이는 노드에는 4종류가 있다.

	|종류|역할|
	|:-------- |:------ |
	| 문서노드(Document Node) | 트리의 최상위, 시작점으로 각 하위요소들에 접근 시 문서 노드를 통해야 함 |
	| 요소노드(Element Node)   | 태그 그 자체를 의미 |
	| 어트리뷰트노드(Attribute Node)   | 어떤 태그 안에 쓰이는 name, value등의 속성 |
	| 텍스트노드(Text Node)   | 태그 내에 기록된 내용으로 텍스트 노드가 존재하는 요소(한 쌍)(div, h1, a, p, li...)와 존재하지 않는 요소(input, img)가 있다 |	

<br>

 3. BOM(Browser Object Model)
	- 자바스크립트와 브라우저가 소통하기 위한 브라우저 객체

	|종류|역할|
	|:-------- |:------ |
	| navigator | 브라우저명과 버전정보를 가짐 |
	| loation | 현재 URL에 대한 정보 |
	| history | 현재 브라우저가 접근했던 URL history |
	| screen | 브라우저의 외부환경에 대한 정보 |	