<script>
  import { onMount } from 'svelte';
  import Icon from '@iconify/svelte';
  import { Avatar } from '@skeletonlabs/skeleton';

  let showIcon = false;

  onMount(() => {
    showIcon = true;
  });
</script>
<div class="container ml-[230px]">
	<form class="max-w-md mx-auto">   
		<label for="default-search" class="mb-2 text-sm font-medium text-gray-900 sr-only dark:text-white">Search</label>
		<div class="relative">
			<div class="absolute inset-y-0 start-0 flex items-center ps-3 pointer-events-none">
				<svg class="w-4 h-4 text-gray-500 dark:text-gray-400" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
					<path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"/>
				</svg>
			</div>
			<input type="search" id="default-search" class="block w-full p-4 ps-10 text-sm text-gray-900 border border-gray-300 rounded-lg bg-gray-50 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="Search items..." required />
			<button type="submit" class="text-white absolute end-2.5 bottom-2.5 bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-4 py-2 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Search</button>
		</div>
	</form>
	<!-- ユーザー名表示 -->
	<div class="flex items-center">
		<Avatar src="https://i.pravatar.cc/" class="w-[48px]"/>
		<h3 class="h3 mt-[15px] ml-[15px]">Motoki Fuki</h3>
	</div>
</div>

<div class="container mx-auto p-8 space-y-8 ml-[230px] flex gap-5">
	<!--記事コンテナ(左)-->
	<div class="w-1/2">
		<!-- 記事題名 -->
		<div class="flex items-center mb-2.5">
			<h2 class="h2">Hello World from Skeleton!</h2>
		</div>
		<!-- コンテンツ本体 -->
		<div class="container">
			<img src="src/image/yz25.jpg" class="u-max-full-width">
		</div>
		<div class="container">
			<p>Hello World!! THis is a sample page!</p>
			<p>And the bike above is my favorite bike.</p>
			<p>This Fz25 is a bike made by YAMAHA, but the vehicle was manufactured in a factory in India.</p>
		</div>

		<button class="my-0"><Icon icon="mdi:cards-heart" width="24" height="24" style="color:red;" /></button>
		<button class="my-0"><Icon icon="mdi:twitter-retweet" width="24" height="24" style="color:green;" /></button>

		<section>
			<a class="btn variant-filled-primary" href="https://kit.svelte.dev/">SvelteKit</a>
			<a class="btn variant-filled-secondary" href="https://tailwindcss.com/">Tailwind</a>
			<a class="btn variant-filled-tertiary" href="https://github.com/">GitHub</a>
		</section>
		{#if showIcon}
		<button><Icon icon="mdi:twitter" width="36" height="36" /></button>
		<button><Icon icon="mdi:instagram" width="36" height="36" /></button>
		<button><Icon icon="mdi:facebook" width="36" height="36" /></button>
		<button><Icon icon="mdi:external-link" width="36" height="36" /></button>
		{/if}
	</div>
	<!--記事コンテナ(右)-->
	<div class="w-1/2 my-0">
		<!-- 記事題名 -->
		<div class="flex items-center mb-2.5">
			<h2 class="h2">Hello World from Skeleton!</h2>
		</div>
		<!-- コンテンツ本体 -->
		<div class="container">
			<img src="src/image/SR400.jpg" class="u-max-full-width">
		</div>
		<div class="container">
			<p>And this bike is an SR400, which I rode when I was a college student.</p>
			<p>I bought a used and battered vehicle, and it was a good bike with engine power,</p>
			<p>although it broke down easily...</p>
		</div>

		<button class="my-0"><Icon icon="mdi:cards-heart" width="24" height="24" style="color:red;" /></button>
		<button class="my-0"><Icon icon="mdi:twitter-retweet" width="24" height="24" style="color:green;" /></button>

		<section>
			<a class="btn variant-filled-primary" href="https://kit.svelte.dev/">SvelteKit</a>
			<a class="btn variant-filled-secondary" href="https://tailwindcss.com/">Tailwind</a>
			<a class="btn variant-filled-tertiary" href="https://github.com/">GitHub</a>
		</section>

		{#if showIcon}
			<button><Icon icon="mdi:twitter" width="36" height="36" /></button>
			<button><Icon icon="mdi:instagram" width="36" height="36" /></button>
			<button><Icon icon="mdi:facebook" width="36" height="36" /></button>
			<button><Icon icon="mdi:external-link" width="36" height="36" /></button>
		{/if}
	</div>
</div>
