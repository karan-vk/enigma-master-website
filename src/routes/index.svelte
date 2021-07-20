<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from "$lib/Counter.svelte";
	import PeopleCard from "$lib/PeopleCard.svelte";
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section class="heroSection">
	<h1>
		<span>w</span>
		<span>e</span>
		<span>l</span>
		<span>c</span>
		<span>o</span>
		<span>m</span>
		<span>e</span>
		<span>&ensp;</span>
		<span>t</span>
		<span>o</span>
		<span>&ensp;</span>
		<span>e</span>
		<span>n</span>
		<span>i</span>
		<span>g</span>
		<span>m</span>
		<span>a</span>
	</h1>
</section>

<section>
	<h2>
		<span>You might ask who we are !</span>
	</h2>
	<p>
		We are a small college group of students who are building a collective
		intelligence to become the best in our field. We have worked on several
		projects and we are now working on a new one aiming to make the world a
		better place.
	</p>
</section>

<section>
	<h1>Meet our team</h1>

	<PeopleCard />
</section>

<style>
	/* section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	} */

	/* .welcome {
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	} */
	@import url(https://fonts.googleapis.com/css?family=Raleway:600);
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		font-family: "Raleway", sans-serif;
	}
	h2 {
		text-align: center;
		font-size: large;
		padding: 1rem;
	}
	p {
		text-indent: 1.5rem;
		padding: 1rem;
	}
	.heroSection {
		width: 100%;
		height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	h1 {
		color: #443860;
		font-family: "Raleway", sans-serif;
		font-size: 52px;
		font-weight: 600;
		text-transform: uppercase;
	}
	h1 span {
		display: inline-block;
		opacity: 0;
		transform: translateY(20px) rotate(90deg);
		transform-origin: left;
		animation: in 0.5s forwards;
	}
	h1 span:nth-child(1) {
		animation-delay: 0.1s;
	}
	h1 span:nth-child(2) {
		animation-delay: 0.2s;
	}
	h1 span:nth-child(3) {
		animation-delay: 0.3s;
	}
	h1 span:nth-child(4) {
		animation-delay: 0.4s;
	}
	h1 span:nth-child(5) {
		animation-delay: 0.5s;
	}
	h1 span:nth-child(6) {
		animation-delay: 0.6s;
	}
	h1 span:nth-child(7) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(8) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(9) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(10) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(11) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(12) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(13) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(14) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(15) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(16) {
		animation-delay: 0.7s;
	}
	h1 span:nth-child(17) {
		animation-delay: 0.7s;
	}

	@keyframes in {
		0% {
			opacity: 0;
			transform: translateY(50px) rotate(90deg);
		}
		100% {
			opacity: 1;
			transform: translateY(0) rotate(0);
		}
	}
</style>
