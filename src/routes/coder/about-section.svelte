<section
	id="about"
	class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24"
	aria-label="About me"
>
	<div
		class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
	>
		<h2 class="text-sm font-bold uppercase tracking-widest text-slate-200 lg:sr-only">About</h2>
	</div>
	<div>
		<p class="mb-4">
			Total 6+ years exp. Senior Software Engineer with a proven track record of driving customer
			acquisition and simplifying processes. Increased onboarding rate by 33% in 1 year. Built
			scalable backends, automated data syncs for customer support, created live call transcription,
			and modernized web chat app with 0 downtime in 6 months.
		</p>

		<p class="mb-6">
			Presently in pursuit of an enriching opportunity within fullstack or frontend development,
			harnessing modern technolody stacks to drive impactful solutions. Eager to
			contribute my expertise in designing and implementing scalable systems, optimizing user
			experiences, and leading collaborative efforts towards innovation and success.
		</p>

		<div class="">

			<h2 class="text-sm font-bold uppercase tracking-widest text-slate-200">Skills</h2>
				<ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
					{#each ['Kotlin', 'JavaScript', 'TypeScript', 'Python', 'Flutter', 'Dart', 'C#', 'Node', 'React', 'Angular', 'Svelte', 'jQuery', 'Redux', 'Django', 'Flask', '.NET', 'Postgres', 'Mongo', 'MySql', 'GraphQL', 'SQLite', 'AWS', 'GCP', 'Cloud Computing', 'CI/CD', 'Cypress', 'Linode', 'Netlify', 'Github/GitLab', 'Jenkins', 'Unit Testing', 'Lambda', 'OOP', 'SaaS', 'PaaS', 'Microservices', 'Distributed Systems', 'Frontend', 'Backend', 'Full-Stack', 'Collaborative', 'Problem Solving', 'English'] as tech}
						<li class="mr-1.5 mt-2">
							<div
								class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
							>
								{tech}
							</div>
						</li>
					{/each}
				</ul>
		</div>

		
	</div>
</section>
