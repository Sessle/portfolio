<script>
	import Project from '$lib/Project.svelte';
	import { clipboard } from '@skeletonlabs/skeleton';

	const discord = ".ses";
	const email = "sethlee1997@gmail.com";
</script>

<div class="container h-full w-1/2 mx-auto flex flex-col space-y-16 justify-center items-center my-16">

	<!-- Me -->
	<div class="card w-full">
		<header class="card-header p-12 pb-6 bg-teal-500 rounded-t-2xl text-center">
			<h1 class="h1">Hello, I'm Seth.</h1>
			<h3 class="h3">Full stack developer.</h3>
		</header>
		<section class="p-4 bg-teal-600 rounded-b-2xl">
			<div class="flex flex-row space-x-2 justify-evenly items-center">
				<a href="https://github.com/Sessle">
					<i class="fa-brands fa-github fa-2xl"></i>
				</a>
				<i class="fa-brands fa-discord fa-2xl cursor-pointer" title="Click to copy" use:clipboard={discord}></i>
				<i class="fa-solid fa-envelope fa-2xl cursor-pointer" title="Click to copy" use:clipboard={email}></i>
			</div>
		</section>
	</div>

	<!-- Skills -->
	<div class="card w-full">
		<header class="card-header p-3 bg-amber-600 rounded-t-2xl text-center">
			<h3 class="h3">Skills</h3>
		</header>
		<section class="p-4 bg-amber-700 rounded-b-2xl">
			<div class="flex flex-row space-x-2 justify-evenly items-center">
				<i class="fa-brands fa-html5 fa-2xl" title="HTML5"></i>
				<i class="fa-brands fa-css3-alt fa-2xl" title="CSS3"></i>
				<i class="fa-brands fa-square-js fa-2xl" title="Javascript"></i>
				<i class="fa-brands fa-node-js fa-2xl" title="NodeJS"></i>
				<img src="/icons/svelte.png" class="w-[34px] h-[34px]" alt="Svelte" title="Svelte"/>
				<img src="/icons/kotlin.png" class="w-[34px] h-[34px]" alt="Kotlin" title="Kotlin"/>
				<img src="/icons/tailwindcss.png" class="w-[55px] h-[34px]" alt="Tailwindcss" title="Tailwindcss"/>
				<img src="/icons/expressjs.png" class="w-[34px] h-[34px]" alt="Expressjs" title="Expressjs"/>
				<img src="/icons/mongodb.png" class="w-[34px] h-[34px]" alt="MongoDB" title="MongoDB"/>
			</div>
		</section>
		<!--<footer class="card-footer">(footer)</footer>-->
	</div>

	<!-- Projects -->
	<div class="card w-full">
		<header class="card-header p-3 bg-red-600 rounded-t-2xl text-center">
			<h3 class="h3">Projects</h3>
		</header>
		<section class="p-4 bg-red-700 rounded-b-2xl">
			<div class="flex flex-col space-y-8 p-2">

				<Project name="AniDatabase" description="A database of anime and their characters, staff, and voice actors." url="https://animelist-frontend.vercel.app/">
					<img src="/icons/svelte.png" class="w-[34px] h-[34px]" alt="Svelte" title="Svelte"/>
					<i class="fa-brands fa-node-js fa-2xl" title="NodeJS"></i>
					<img src="/icons/fastify.png" class="w-[52px] h-[33px]" alt="Fastify" title="Fastify"/>
					<img src="/icons/postgresql.png" class="w-[34px] h-[34px]" alt="Postgresql" title="Postgresql"/>
				</Project>

				<Project name="RuneIdle" description="An MMO idle game inspired by RuneScape." url="https://runeidle.com">
					<img src="/icons/svelte.png" class="w-[34px] h-[34px]" alt="Svelte" title="Svelte"/>
					<i class="fa-brands fa-node-js fa-2xl" title="NodeJS"></i>
					<img src="/icons/expressjs.png" class="w-[34px] h-[34px]" alt="Expressjs" title="Expressjs"/>

					<img src="/icons/kotlin.png" class="w-[34px] h-[34px]" alt="Kotlin" title="Kotlin"/>
					<img src="/icons/mongodb.png" class="w-[34px] h-[34px]" alt="MongoDB" title="MongoDB"/>
				</Project>

				<Project name="Latte Calculator" description="A calculator for making lattes with pour-over coffee." url="https://lattecalculator.vercel.app/">
					<img src="/icons/svelte.png" class="w-[34px] h-[34px]" alt="Svelte" title="Svelte"/>
				</Project>

			</div>
		</section>
	</div>
</div>
