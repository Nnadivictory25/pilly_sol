<script>
	import { fade } from 'svelte/transition';
	import { onMount } from 'svelte';
	let ca = 'F9Np8S8xYdNuDEgtFHiYfqYh3V1QMawueuvvhUGapump';
	let animate = false;
    

	function copyCA() {
		try {
			navigator.clipboard.writeText(ca);
			alert('CA Copied to clipboard');
		} catch (err) {
			alert('Failed to copy');
		}
	}

	onMount(() => {
		animate = true;
	});
</script>



<div class="grid justify-center px-10 pt-5">
	<h1 class="text-xl font-extrabold">Did you miss $PEPE ?</h1>
	<h1 class="text-xl font-extrabold">Did you also miss $BILLY ?</h1>

	<h1 class="mt-4 text-2xl font-extrabold">Then $PEPILLY is for you</h1>

	<div class="mt-10 flex flex-wrap items-center justify-center gap-5 md:gap-10">
		<div class="md:h-[200px] md:w-[200px]">
			{#if animate}
				<img
					in:fade={{ duration: 1000 }}
					src="/pepe.png"
					alt="pepe"
					class="h-28 w-28 rounded-lg md:h-[200px] md:w-[200px]"
					width="200"
					height="200"
				/>
			{/if}
		</div>
		<span class="text-3xl font-extrabold">+</span>
		<div class="md:h-[200px] md:w-[200px]">
			{#if animate}
				<img
					in:fade={{ duration: 1000, delay: 500 }}
					src="/billy.webp"
					alt="billy"
					class="h-28 w-28 rounded-lg md:h-[200px] md:w-[200px]"
					width="200"
					height="200"
				/>
			{/if}
		</div>
		<span class="text-3xl font-extrabold">=</span>
		<div class="md:h-[200px] md:w-[200px]">
			{#if animate}
				<img
					in:fade={{ duration: 1000, delay: 1000 }}
					src="/pilly.jpg"
					alt="pilly"
					class="h-28 w-28 rounded-lg md:h-[200px] md:w-[200px]"
					width="200"
					height="200"
				/>
			{/if}
		</div>
	</div>

	<p class="mt-8 text-center font-bold">ARE YOU GONNA FADE ?</p>

	<div
		class="md:text-md mx-auto mt-10 flex items-center justify-center gap-3 rounded-md border-2 p-3 text-sm font-bold md:w-fit"
	>
		<p class="w-[230px] overflow-hidden text-ellipsis md:w-auto">
			CA : F9Np8S8xYdNuDEgtFHiYfqYh3V1QMawueuvvhUGapump
		</p>

		<button on:click={() => copyCA()} class="rounded-md bg-green-500 p-4">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="24"
				height="24"
				viewBox="0 0 24 24"
				fill="none"
				stroke="currentColor"
				stroke-width="2"
				stroke-linecap="round"
				stroke-linejoin="round"
				class="lucide lucide-copy cursor-pointer hover:text-gray-400"
				><rect width="14" height="14" x="8" y="8" rx="2" ry="2" /><path
					d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"
				/></svg
			>
		</button>
	</div>

	<div class="mt-5 flex items-center justify-center gap-7">
		<a
			class="transition-all hover:opacity-80"
			href="https://www.pump.fun/F9Np8S8xYdNuDEgtFHiYfqYh3V1QMawueuvvhUGapump"
			target="_blank"
		>
			<img src="/pumpfun.jpg" alt="pump.fun" class="rounded-full" width="50" height="50" />
		</a>

		<a
			class="transition-all hover:opacity-80"
			href="https://dexscreener.com/solana/F9Np8S8xYdNuDEgtFHiYfqYh3V1QMawueuvvhUGapump"
			target="_blank"
		>
			<img src="/dexscreener.png" alt="dexscreener" class="rounded-full" width="50" height="50" />
		</a>

		<a class="transition-all hover:opacity-80" href="https://x.com/pepillyonsol" target="_blank">
			<img src="/x.jpg" alt="X" class="rounded-full" width="50" height="50" />
		</a>

		<a class="transition-all hover:opacity-80" href="https://t.me/PEPILLYSOL" target="_blank">
			<img src="/telegram.png" alt="X" class="rounded-full" width="50" height="50" />
		</a>
	</div>
</div>

<style>
	h1 {
		text-align: center;
	}

	img {
		@apply border-2 border-white;
	}
</style>
