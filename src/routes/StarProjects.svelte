<script>
	import FleetLogo from '$lib/images/fleet_logo.png';
</script>

<div>
	<h1 class="text-xl font-light mb-6 lg:text-3xl">Featured projects</h1>
	<h1 class="font-bold text-5xl lg:text-8xl lg:mb-16 mb-3">Fleet ⚡️</h1>
	<div class="lg:grid lg:grid-cols-6 lg:gap-14">
		<img src={FleetLogo} class="rounded-lg lg:hidden" />
		<div class="lg:col-span-4">
			<p class="my-6 lg:my-0 lg:text-xl text-lg">
				Being my first real world project, with real users and meaningful impact in their lives,
				Fleet is a project that I'm very proud of.<br /><br />
				Fleet is a 100% free application that provides real-time information on the results of current,
				past and future athletics competitions in Portugal.<br /><br /> It also provides information
				on Portuguese athletics clubs and athletes.
			</p>
			<button
				class="block lg:text-lg lg:mt-8 text-white hover:text-[#151518] hover:bg-white hover:outline-none hover:ring-blue-300 font-medium rounded-lg text-sm px-3 py-1.5 text-center border"
				><a
					href="https://play.google.com/store/apps/details?id=com.fleet_athletics01.app&hl=pt_PT"
					target="_blank">See more...</a
				></button
			>
		</div>
		<img src={FleetLogo} class="rounded-lg lg:col-span-2 hidden lg:block" />
	</div>
</div>
