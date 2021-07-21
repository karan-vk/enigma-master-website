<script>
	export let people = [
		{
			name: "Karan",
			designation: "Backend Dev | AI Engineer",
			heroImage: "",
			heroImageUrl: "https://i.ibb.co/bmzzjTR/new-dp.png",
			Text: "Going with a rusting life is my motto and everything that I do prevails",
			joinMonth: "Dec",
			joinYear: "2019",
			slug: "karan",
		},
		{
			name: "Sathish",
			designation: "Developer | AI Engineer",
			heroImage: "",
			heroImageUrl: "https://avatars.githubusercontent.com/u/54014069?v=4",
			Text: "I can make your data into stories",
			joinMonth: "Dec",
			joinYear: "2019",
		},
		{
			name: "Vishal ",
			designation: "Developer | AI Engineer",
			heroImage: "",
			heroImageUrl: "https://i.ibb.co/6BqkMSS/photo-2021-07-21-20-14-37.jpg",
			Text: "AI & ML Enthusiast (SS)",
			joinMonth: "Jan",
			joinYear: "2020",
		},
	];
</script>

<div class="row">
	{#each people as person}
		<div class="example-2 card">
			<div
				class="wrapper"
				style="background: url({person.heroImageUrl})center / cover no-repeat ;"
			>
				<div class="header">
					<div class="date">
						<!-- <span class="day">12</span> -->
						<span class="month">{person.joinMonth}</span>
						<span class="year">{person.joinYear}</span>
					</div>
				</div>
				<div class="data">
					<div class="content">
						<!-- <span class="author">Jane Doe</span> -->
						<h1 class="title">
							<a href={person.slug}>{person.name}</a>
							<p>{person.designation}</p>
						</h1>
						<p class="text">
							{person.Text}
						</p>
						<a href={person.slug} class="button">How you doin</a>
					</div>
				</div>
			</div>
		</div>
	{/each}
</div>

<style>
	@import url(https://fonts.googleapis.com/css?family=Open+Sans:300,400,700);
	* {
		box-sizing: border-box;
	}

	a {
		text-decoration: none;
	}
	h1 {
		font-family: "Open Sans", sans-serif;
		font-weight: 300;
	}
	.row {
		max-width: 900px;
		margin: 50px 50px 0;
	}
	.card {
		float: left;
		padding: 0 1.7rem;
		width: 50%;
	}

	.card .menu-content a {
		color: #fff;
	}
	.card .menu-content span {
		position: absolute;
		left: 50%;
		top: 0;
		font-size: 10px;
		font-weight: 700;
		font-family: "Open Sans";
		transform: translate(-50%, 0);
	}
	.card .wrapper {
		background-color: #fff;
		min-height: 540px;
		position: relative;
		overflow: hidden;
		box-shadow: 0 19px 38px rgba(0, 0, 0, 0.3), 0 15px 12px rgba(0, 0, 0, 0.2);
	}
	.card .wrapper:hover .data {
		transform: translateY(0);
	}
	.card .data {
		position: absolute;
		bottom: 0;
		width: 100%;
		transform: translateY(calc(70px + 1em));
		transition: transform 0.3s;
	}
	.card .data .content {
		padding: 1em;
		position: relative;
		z-index: 1;
	}

	.card .title {
		margin-top: 10px;
	}
	.card .title p {
		font-size: 1rem;
		color: #fff;
	}
	.card .text {
		color: #fff;
		height: 70px;
		margin: 0;
	}

	.example-2 .wrapper {
		background: url(https://tvseriescritic.files.wordpress.com/2016/10/stranger-things-bicycle-lights-children.jpg)
			center / cover no-repeat;
	}
	.example-2 .wrapper:hover .menu-content span {
		transform: translate(-50%, -10px);
		opacity: 1;
	}
	.example-2 .header {
		color: #fff;
		padding: 1em;
	}
	.example-2 .header::before,
	.example-2 .header::after {
		content: "";
		display: table;
	}
	.example-2 .header::after {
		clear: both;
	}
	.example-2 .header .date {
		float: left;
		font-size: 12px;
	}

	.example-2 .menu-content span {
		transition: all 0.3s;
		opacity: 0;
	}
	.example-2 .data {
		color: #fff;
		transform: translateY(calc(70px + 4em));
	}
	.example-2 .title a {
		color: #fff;
	}
	.example-2 .button {
		display: block;
		width: 100px;
		margin: 2em auto 1em;
		text-align: center;
		font-size: 12px;
		color: #fff;
		line-height: 1;
		position: relative;
		font-weight: 700;
	}
	.example-2 .button::after {
		content: "\2192";
		opacity: 0;
		position: absolute;
		right: 0;
		top: 50%;
		transform: translate(0, -50%);
		transition: all 0.3s;
	}
	.example-2 .button:hover::after {
		transform: translate(5px, -50%);
		opacity: 1;
	}
</style>
