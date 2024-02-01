<!-- <script>
	let m = { x: 0, y: 0};

	function handleMousemove(event) {
		m.x = event.clientX;
		m.y = event.clientY;
	}
</script>

<div on:mousemove={handleMousemove}>
	The mouse position is {m.x} x {m.y}
</div>

<style>
	div {
		width: 100%;
		height: 100%;
	}
</style> 
기본이벤트
-->

<!-- <script>
	let m = { x: 0, y: 0};
</script>

<div on:mousemove="{e => m = { x: e.clientX, y: e.clientY }}">
	The mouse position is {m.x} x {m.y}
</div>

<style>
	div {
		width: 100%;
        height: 100%;
	}
</style>
인라인 이벤트
전달인자 있으면 인라인 이벤트를 사용해야함
-->

<script>
	function handleClick() {
		alert('no more alerts')
	}
</script>

<button on:click|once={handleClick}>
	Click me
</button>

<!-- 
	이벤트들
마우스 이벤트
	- click: 사용자가 마우스를 클릭했을 때
	- dblclick: 사용자가 마우스를 더블클릭했을 때
	- mousedown: 사용자가 마우스를 누르고 있을 때
	- mouseu: 눌렀던 마우스에서 손을 뗄 때
	- mousemove: 마우스를 움직일때
	- mouseover: 특정 요소 위로 마우스를 움직였을때

키보드 이벤트
    - keydown: 사용자가 키를 처음 눌렀을 때
	- keyup: 눌렀던 키에서 손을 뗄 때
	- keypress: 눌렀던 키의 문자가 입력되었을 때

기타 이벤트
    - scroll: 페이지 스크롤이 발생했을 때
	- resize: 브라우저 창 크기가 변경되었을 때
-->

<!-- 수식어들

	- preventDefault:

-->