<script>
	import CreateEventButton from './CreateEventButton.svelte';
	import LoginButton from './LoginButton.svelte';
</script>

<header>
	<h1>
		<a href="/">Plus Mate</a>
	</h1>

	<nav>
		<ul>
			<li>
				<a href="/about">
					<p>PlusMateとは</p>
				</a>
			</li>
			<li>
				<a href="/following">
					<p>フォロー中</p>
				</a>
			</li>
			<li>
				<CreateEventButton />
			</li>
			<li>
				<LoginButton />
			</li>
		</ul>
	</nav>
</header>

<style>
	header {
		padding: 24px 40px;
		display: flex;
		align-items: center;
		justify-content: space-between;

		border-bottom: solid 1px black;
	}

	h1>a {
		font-size: 32px;
		color: black;
		font-weight: 300;
		text-decoration: none;
	}
	
	nav>ul {
		list-style: none;
		display: flex;
		align-items: center;
		gap: 32px;
	}

	li>a>p {
		font-size: 20px;
	}
</style>
