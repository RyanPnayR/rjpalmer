<script lang="ts">
	import ProjectCard from '$lib/components/ui/project-card/project-card.svelte';
	import smiles from '$lib/assests/images/rob-smiles-website.png';
</script>

<section
	id="projects"
	class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24"
	aria-label="Selected projects"
>
	<div
		class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
	>
		<h2 class="text-sm font-bold uppercase tracking-widest text-slate-200 lg:sr-only">Projects</h2>
	</div>
	<div>
		<ul class="group/list">
			<li class="mb-12">
				<ProjectCard
					link="https://www.robsmilescomedy.com"
					title="Custom Squarespace Website"
					description="Designed and created a responsive squarespace website for headlining comedian RobSmiles. I created all the visual components, the design, and the theme. I created a custom map and voting form to gather fan interest for future shows, merch and email marketing. I tought the comedians team how to manage his site for his merch, show dates, and email campaigns. "
					photoSrcSet="{smiles} 500w, {smiles} 1000w, {smiles} 2000w"
          technologies={["SquareSpace", "React", "Next.js", "Vercel", "AWS", "Sendgrid"]}
				/>
			</li>
		</ul>
		<!-- <div class="mt-12">
    <a
      class="group inline-flex items-center font-medium font-semibold leading-tight text-slate-200 text-slate-200"
      aria-label="View Full Project Archive"
      href="/archive"
      ><span
        ><span
          class="border-b border-transparent pb-px transition group-hover:border-teal-300 motion-reduce:transition-none"
          >View Full Project
        </span><span class="whitespace-nowrap"
          ><span
            class="border-b border-transparent pb-px transition group-hover:border-teal-300 motion-reduce:transition-none"
            >Archive</span
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 20 20"
            fill="currentColor"
            class="ml-1 inline-block h-4 w-4 shrink-0 -translate-y-px transition-transform group-hover:translate-x-2 group-focus-visible:translate-x-2 motion-reduce:transition-none"
            aria-hidden="true"
          >
            <path
              fill-rule="evenodd"
              d="M3 10a.75.75 0 01.75-.75h10.638L10.23 5.29a.75.75 0 111.04-1.08l5.5 5.25a.75.75 0 010 1.08l-5.5 5.25a.75.75 0 11-1.04-1.08l4.158-3.96H3.75A.75.75 0 013 10z"
              clip-rule="evenodd"
            ></path>
          </svg></span
        ></span
      ></a
    >
  </div> -->
	</div>
</section>
