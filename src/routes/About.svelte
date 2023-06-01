<script lang="ts">
	import profile from '$lib/images/profile_pic.jpg';
	import CV from '$lib/assets/CV_en.pdf';
</script>

<div class=" pt-6 lg:grid lg:grid-cols-6 lg:gap-10" id="about">
	<div class="lg:col-span-4">
		<div class="relative mb-16">
			<hr class="w-full h-px my-8 bg-gray-200 border-0 dark:bg-gray-700" />
			<span
				class="absolute pr-3 font-bold text-white text-4xl lg:text-6xl bg-[#151518] left-0 top-0 -translate-y-1/2"
				>About Me</span
			>
		</div>
		<p class="lg:text-xl">
			I am a Software Engineering Student. Interested in programming and software engineering. I
			like sports, mainly athletics and basketball and I am passionate about photography and
			videography.
			<br /><br />
			Currently I am getting my master's degree in Software Engineering at the University of Porto, mainly
			focusing on the areas of Software Engineering and Product Management and the area of Machine Learning
			and Artificial Intelligence.
			<br /><br />
			You might find me often working on some side projects, learning new technologies and launching
			new products.
		</p>
	</div>
	<div class="lg:col-span-2">
		<div class="w-full flex justify-center ">
			<img src={profile} class="pt-14 lg:pt-0 lg:w-full w-4/5" alt="" />
		</div>
		<div class="lg:flex lg:justify-end">
			<button
				class="mt-10 inline-flex items-center px-3 py-2 text-sm font-medium lg:text-lg text-center text-white bg-indigo-600 rounded-lg hover:bg-indigo-800 focus:ring-4 focus:outline-none focus:ring-blue-300 "
			>
				<a href={CV} download>Download my CV</a>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					height="1em"
					viewBox="0 0 512 512"
					class="w-4 h-4 ml-2 -mr-1 lg:w-5 lg:h-5"
					fill="currentColor"
					><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path
						d="M288 32c0-17.7-14.3-32-32-32s-32 14.3-32 32V274.7l-73.4-73.4c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3l128 128c12.5 12.5 32.8 12.5 45.3 0l128-128c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0L288 274.7V32zM64 352c-35.3 0-64 28.7-64 64v32c0 35.3 28.7 64 64 64H448c35.3 0 64-28.7 64-64V416c0-35.3-28.7-64-64-64H346.5l-45.3 45.3c-25 25-65.5 25-90.5 0L165.5 352H64zm368 56a24 24 0 1 1 0 48 24 24 0 1 1 0-48z"
					/></svg
				>
			</button>
		</div>
	</div>
</div>
