<script>
	import AppCard from './AppCard.svelte';
</script>

<section class="px-6 pb-16">
	<div class="max-w-2xl mx-auto">
		<h2 class="text-[clamp(0.8rem,2vw,1rem)] text-center mb-8 text-text">Apps</h2>
		<div class="flex flex-col gap-6">
			<AppCard
				icon="/crumbs-logo.png"
				name="Crumbs"
				tagline="Thoughtful note-taking"
				description="A self-hosted note-taking app with rich text editing, color-coded notebooks, and offline support. Your notes stay on your server."
				url="https://crumbs.bretzel.app"
				githubUrl="https://github.com/bretzel-app/crumbs"
			/>
			<AppCard
				icon="/42-logo.png"
				name="42"
				tagline="Holiday budget tracking"
				description="A self-hosted trip budget tracker with multi-currency support, real-time spending analytics, and offline sync. Your trips, your budget, your rules."
				url="https://42.bretzel.app"
				githubUrl="https://github.com/bretzel-app/42"
			/>
		</div>
	</div>
</section>
