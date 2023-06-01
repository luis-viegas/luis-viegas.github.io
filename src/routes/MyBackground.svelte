<script>
	import { Swipe, SwipeItem } from 'svelte-swipe';
	const swipeConfig = {
		autoplay: false,
		showIndicators: true,
		transitionDuration: 200,
		defaultIndex: 0
	};
</script>

<div class="w-full flex justify-center" id="background">
	<h1 class="text-3xl font-bold my-4 lg:text-6xl lg:mb-20">My background</h1>
</div>
<div class="max-w-sm px-6 pb-2 pt-6 bg-[#2a2a2a] lg:hidden   rounded-lg shadow">
	<div class="swipe-holder">
		<Swipe {...swipeConfig}>
			<SwipeItem>
				<h2 class="font-bold text-xl pb-1">Side work</h2>
				<p class="text-xs text-gray-200 pb-3">2020 - Present</p>
				<ul class="max-w-md space-y-6  text-gray-200 list-inside text-sm">
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Several personal websites and projects for clients. Including an icon editing web app and
						multiple personal websites.
					</li>
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Developed the largest platform for Portuguese Athletics Information with excellent reception
						from te public and various Portuguese athletics associations.
					</li>
				</ul>
			</SwipeItem>

			<SwipeItem>
				<h2 class="font-bold text-xl pb-1">
					University - Masters in Software Engineering <a
						href="https://sigarra.up.pt/feup/en/web_base.gera_pagina?p_pagina=1182"
						class="font-medium text-indigo-400">@FEUP</a
					>
				</h2>
				<p class="text-xs text-gray-200 pb-3">2019 - 2024</p>
				<ul class="max-w-md space-y-6  text-gray-200 list-inside text-sm">
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Bsc in Software Engineering from 2019 to 2022.
					</li>
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Masters in Software Engineering from 2022 to 2024.
					</li>
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Spent one semester abroad in Croatia at the University of Zagreb.
					</li>
				</ul>
			</SwipeItem>

			<SwipeItem>
				<h2 class="font-bold text-xl pb-1">
					High School <span class="font-medium text-indigo-400"
						>@Escola Secundária do Castêlo da Maia</span
					>
				</h2>
				<p class="text-xs text-gray-200 pb-3">2016 - 2019</p>
				<ul class="max-w-md space-y-6  text-gray-200 list-inside text-sm">
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Part of the school's best students dinstinction every year.
					</li>
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Vice-president of the students association. Responsible for the organization of events and
						prom party.
					</li>
					<li class="flex items-start">
						<svg
							class="w-4 h-4 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
						>
							<path
								fill-rule="evenodd"
								d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
								clip-rule="evenodd"
							/>
						</svg>
						Participated on several Physics and Maths competitions, winning the 1st place on the regional
						maths competition.
					</li>
				</ul>
			</SwipeItem>
		</Swipe>
	</div>
</div>

<div>
	<div class="hidden lg:block lg:mb-20">
		<h2 class="font-bold text-3xl pb-1">
			High School <span class="font-medium text-indigo-400"
				>@Escola Secundária do Castêlo da Maia</span
			>
		</h2>
		<p class="text-xs lg:text-lg text-gray-200 pb-3">2016 - 2019</p>
		<ul class="max-w-md space-y-6  text-gray-200 list-inside text-sm">
			<li class="flex lg:text-lg  items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Part of the school's best students dinstinction every year.
			</li>
			<li class="flex lg:text-lg  items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Vice-president of the students association. Responsible for the organization of events and prom
				party.
			</li>
			<li class="flex lg:text-lg  items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Participated on several Physics and Maths competitions, winning the 1st place on the regional
				maths competition.
			</li>
		</ul>
	</div>
	<div class="hidden lg:block lg:mb-20">
		<h2 class="font-bold text-3xl pb-1">
			University - Masters in Software Engineering <a
				href="https://sigarra.up.pt/feup/en/web_base.gera_pagina?p_pagina=1182"
				class="font-medium text-indigo-400">@FEUP</a
			>
		</h2>
		<p class="text-xs  lg:text-lg text-gray-200 pb-3">2019 - 2024</p>
		<ul class="max-w-md space-y-6  text-gray-200 list-inside text-sm">
			<li class="flex  lg:text-lg items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Bsc in Software Engineering from 2019 to 2022.
			</li>
			<li class="flex  lg:text-lg items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Masters in Software Engineering from 2022 to 2024.
			</li>
			<li class="flex  lg:text-lg items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Spent one semester abroad in Croatia at the University of Zagreb.
			</li>
		</ul>
	</div>
	<div class="hidden lg:inline">
		<h2 class="font-bold text-3xl pb-1">Side work</h2>
		<p class="text-xs lg:text-xl text-gray-200 pb-3">2020 - Present</p>
		<ul class="max-w-md space-y-6  text-gray-200 list-inside text-sm">
			<li class="flex lg:text-xl items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Several personal websites and projects for clients. Including an icon editing web app and multiple
				personal websites.
			</li>
			<li class="flex lg:text-xl items-start">
				<svg
					class="w-4 h-4 lg:w-6 lg:h-6 mr-1.5 mt-1 text-indigo-400 flex-shrink-0"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path
						fill-rule="evenodd"
						d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z"
						clip-rule="evenodd"
					/>
				</svg>
				Developed the largest platform for Portuguese Athletics Information with excellent reception
				from te public and various Portuguese athletics associations.
			</li>
		</ul>
	</div>
</div>

<style>
	.swipe-holder {
		height: 30rem;
		width: 100%;
	}
	img {
		max-width: 100%;
		height: auto;
	}
</style>
