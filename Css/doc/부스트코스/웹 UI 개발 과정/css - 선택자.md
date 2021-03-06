# css 선택자
##### 1. 부분 속성값으로 선택
	- [class~="bar"]: class 속성의 값이 공백으로 구분한 "bar" 단어가 포함되는 요소 선택<br/>
		- 적용 예) class="color hot" / class="cool color" <br/> 
	- [class^="bar"]: class 속성의 값이 "bar"로 시작하는 요소 선택<br/>
		- 적용 예) class="color hot" / class="colorful nature" <br/>
	- [class$="bar"]: class 속성의 값이 "bar"로 끝나는 요소 선택<br/>
		- 적용 예) class="cool color" <br/>
	- [class*="bar"]: class 속성의 값이 "bar" 문자가 포함되는 요소 선택<br/>
		- 적용 예) class="color hot" / class="cool color" / class="colorful nature" <br/>

##### 2. 문서 구조 관련 선택자
	- 자손 선택자
		- ex) div span { } // div의 자손 span을 선택...
	- 자식 선택자
		- ex) div > span { } // div의 자식 span 선택...
	- 인접 형제 선택자
		- ex) div + span { } // div의 인접한 뒤에 형제를 선택...
		
##### 3. 가상 선택자
	- 가상 클래스
		- 미리 정의해놓은 상황에 적용이 되도록 약속되어있는 보이지 않는 클래스
		- ex) :pseudo-class { property: value; } // 브라우저 스스로가 특정 상황이 되면 자동적으로 클래스를 생성
		- ex) :hover { } 
		- ex) li:first-child { }
		- ex) li:last-child { }
		
	- 가상 요소
		- 미리 정의해놓은 위치에 삽입이 되도록 약속되어있는 보이지 않는 요소
		- ex) p:before{ } 가장 앞에 요소를 삽입 (content 필요)
		- ex) :after: 가장 뒤에 요소를 삽입 (content 필요)
		- ex) :first-line: 요소의 첫 번째 줄에 있는 텍스트
		- ex) :first-letter: 블록 레벨 요소의 첫 번째 문자
		
		
		
##### - position ,offset
	-	position
		- static: 포지션이 static일 경우 top, left 등이 먹지 않는다.
		- relative: 자리를 유지하면서, top, left 만큼 움직인다. 
		- absolute: 부모가 relative면 부모를 기준으로 좌표를 잡는다. 없으면 할아부지.. 없으면 body....
		- fixed: 브라우저를 기준으로 화면 고정... 
		- absolute, fixed의 경우 박스 모델이 block이 된다.
		
		
##### - z-index		 
		- 박스가 겹치는 순서를 정한다.
		- position이 static이 아닌 경우 지정 가능 ( z-index: 1, 2, ...;)
		- 부모가 z-index 값이 있을 경우 부모 안에서만 의미 있다. 
		- (부모-자식) (부모-자식) 중 자식이 다른 자식 보다 z-index가 낮아도 부모의 z-index가 높다면 더 위에 올라온다.
		
		
##### - 미디어 쿼리 (Media Queries)
	- 반응형 웹 사이트를 만들기 위해 반드시 필요한 것..
	- 각 미디어 매체에 따라 다른 스타일 시트를 적용할수 있게 만드는 것
		- 미디어(screen, print, ....)
	
		
[1. 미디어 쿼리 1](https://www.w3.org/TR/css3-mediaqueries/)
[2. 미디어 쿼리 2](https://www.w3.org/TR/mediaqueries-4/)
[3. 미디어 쿼리 3 - 어떤 식으로 반응형 웹 사이트를 구축하는지 .....](https://mediaqueri.es/)

[부스트코스 웹 UI 개발 과정 - 프로젝트 A-1](https://www.edwith.org/boostcourse-ui/joinLectures/19152)

		
		