<script lang="ts">
	import Header from './header-section.svelte';
	import About from './about-section.svelte';
	import Experience from './expierence-section.svelte';
	import Projects from './project-section.svelte';
	import Blog from './blog-section.svelte';
	import Footer from './footer-section.svelte';
</script>

<div
	class="mx-auto min-h-screen max-w-screen-xl px-6 py-12 font-sans md:px-12 md:py-20 lg:px-24 lg:py-0"
>
	<a
		href="#content"
		class="absolute left-0 top-0 block -translate-x-full rounded bg-gradient-to-br from-teal-400 via-blue-500 to-purple-600 px-4 py-3 text-sm font-bold uppercase tracking-widest text-white focus-visible:translate-x-0"
		>Skip to Content</a
	>
	<div class="lg:flex lg:justify-between lg:gap-4">
		<Header />
		<main id="content" class="pt-24 lg:w-1/2 lg:py-24">
			<About />
			<Experience />
			<Projects />
			<Blog />
			<Footer />
		</main>
	</div>
</div>
