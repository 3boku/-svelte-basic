<!-- <script>
	let people = {
		name: "John",
		age: 29,
		sex: "male",
	}
</script>

<h2>이름: {people.name}</h2>
<h2>나이: {people.age}</h2>
<h2>성별: {people.sex}</h2> 
객체형 상태값-->

<script>
	let list = [
		{
			id: 0,
			content: '첫 번쨰 할 일',
			done: false
		},
		{
			id: 1,
			content: '두 번쨰 할 일',
			done: false
		},
		{
			id: 2,
			content: '세 번쨰 할 일',
			done: false
		},
		{
			id: 3,
			content: '네 번쨰 할 일',
			done: false
		}
	]

	const handleAddTodo = () => {
		const todo = {
			id: list.length + 1,
			content: '새로운 할 일',
			done: false
		}
		// list.push(todo);

		// list = list;
		// 재할당해줘야 list가 새로 생김

		list = [...list, todo];
		// 스프레드라고 하는건데 위에꺼랑 같은 기능임
	}

	
</script>

<ul>
	{#each list as item}
		<li>
			<p>{item.content}</p>
		</li>
	{/each}
</ul>

<button on:click={handleAddTodo}>할일 추가</button>
<!--배열형 상태값-->