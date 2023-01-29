<script>
	import '../app.css';
	let isNavOpen = false;
	const toggleNav = () => {
		isNavOpen = !isNavOpen;
	};
</script>

<header class="shadow-md">
	<div class="flex-grow w-full max-w-screen-2xl mx-auto p-4">
		<div class="flex gap-4">
			<a href="/"
				><img src="/images/logo.png" alt="logo" style="width: 26ch;" />
				<div class="text-gray-600">ALL YOUR IT SOLUTION NEEDS</div></a
			>
			<nav class="self-end ml-auto text-gray-800 text-xl flex gap-4 max-md:hidden">
				<a href="/" class="hover:underline">Home</a>
				<a href="/about" class="hover:underline">About</a>
				<a href="/contact" class="hover:underline">Contact Us</a>
			</nav>
			<button class="self-center ml-auto flex flex-col gap-2 md:hidden" on:click={toggleNav}>
				<div class="border-solid border-2 border-black w-8" />
				<div class="border-solid border-2 border-black w-8" />
				<div class="border-solid border-2 border-black w-8" />
			</button>
		</div>
		<nav
			class="flex flex-col items-end md:hidden overflow-hidden {isNavOpen ? 'max-h-24' : 'max-h-0'}"
			style="transition: max-height 350ms ease-out;"
		>
			<a href="/" class="hover:underline h-8 shrink-0">Home</a>
			<a href="/about" class="hover:underline h-8 shrink-0">About</a>
			<a href="/contact" class="hover:underline h-8 shrink-0">Contact Us</a>
		</nav>
	</div>
</header>
<div class="h-full overflow-auto">
	<slot />
</div>
<footer class="max-md:hidden">
	<div class="flex-grow w-full max-w-screen-2xl mx-auto p-4 text-center text-lg">
		<div>2986 Danforth Ave. Suite #205</div>
		<div>M4C 1M6, Toronto, Ontario</div>
		<div class="border-t border-gray-800" />
		<div>&copy; 2023 The IPWorld Inc. All rights reserved.</div>
	</div>
</footer>
