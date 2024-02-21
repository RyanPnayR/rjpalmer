<script lang="ts">
	import TimelineEntryCard from '$lib/components/ui/timeline-entry-card/timeline-entry-card.svelte';
	import resume from '$lib/assests/Resume_Ryan_Palmer.pdf';
</script>

<section
	id="experience"
	class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24"
	aria-label="Work experience"
>
	<div
		class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
	>
		<h2 class="text-sm font-bold uppercase tracking-widest text-slate-200 lg:sr-only">
			Experience
		</h2>
	</div>
	<div>
		<ol class="group/list">
			<li class="mb-12">
				<TimelineEntryCard
					start="2022 Apr"
					end="2023 Mar"
					role="Senior Software Engineer"
					companyName="Level Technology"
					description="Built out modern online banking solutions for gig workers via Plaid,
					Unit, and Argyle. Set up automated syncs for customer support for tools like Zendesk and Hubspot with our private systems."
					technologies={['React', 'Kotlin', 'Python', 'AWS', 'Postgres']}
					companyWebsite="https://www.levelgoals.com"
				></TimelineEntryCard>
			</li>
			<li class="mb-12">
				<TimelineEntryCard
					start="Jul 2021"
					end="Jun 2022"
					role="Senior Software Engineer"
					companyName="Live Person/Tenfold"
					description="Lead a team of engineers to build out Tenfold's Webex phone integration. Developed transcribing live agent calls to Salesforce with a custom integration."
					technologies={['Angular', 'Express', 'Node.js', 'GCP', 'AWS', 'MongoDB']}
					companyWebsite="https://www.tenfold.com"
				></TimelineEntryCard>
			</li>
			<li class="mb-12">
				<TimelineEntryCard
					start="Feb 2019"
					end="Jul 2021"
					role="Full Stack Software Engineer"
					companyName="Redeapp"
					description="Performed web app migration from Angular.js to modern angular and established end too end testing in cypress. Lead Redeapp's Android development by building out, testing, and deploying changes for their messaging platform."
					technologies={['Angular', 'Kotlin', 'Java', 'Python', 'AWS', 'Postgres', 'Android']}
					companyWebsite="https://www.redeapp.com"
				></TimelineEntryCard>
			</li>
			<li class="mb-12">
				<TimelineEntryCard
					start="Jul 2021"
					end="Jun 2022"
					role="Software Engineer"
					companyName="Level 12"
					description="Created new and maintained old web apps for a consulting firm withing strict timeframes and budgets. Maintained product quality by keeping at least 90% automated tests coverage."
					technologies={['Python', 'React', 'Linode', 'SQLAlchemy', 'Postgres']}
					companyWebsite="https://www.level12.io"
				></TimelineEntryCard>
			</li>
			<li class="mb-12">
				<TimelineEntryCard
					start="Aug 2016"
					end="Oct 2017"
					role="Senior Software Engineer"
					companyName="Astronomer"
					description="Created and maintained containerized Node.js integrations and libraries for Astronomers open sourced Analytics.js
					Platform. Designed Airflow data pipelines written in Node.js and python connecting external data sources to databases sending up
					to millions of events with test coverage in Mocha, Chai, and Nock."
					technologies={[
						'Javascript',
						'Express',
						'Node.js',
						'Python',
						'AWS',
						'Postgres',
						'MongoDB',
						'Airflow',
						'Analytics.js'
					]}
					companyWebsite="https://www.Astronomer.io"
				></TimelineEntryCard>
			</li>
		</ol>
		<div class="mt-12">
			<a
				class="group/link inline-flex items-baseline text-base font-medium font-semibold leading-tight text-slate-200 text-slate-200 hover:text-teal-300 focus-visible:text-teal-300"
				href={resume}
				target="_blank"
				rel="noreferrer noopener"
				aria-label="View Full Résumé (opens in a new tab)"
				><span
					>View Full <span class="inline-block"
						>Résumé<svg
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
							class="ml-1 inline-block h-4 w-4 shrink-0 translate-y-px transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none"
							aria-hidden="true"
						>
							<path
								fill-rule="evenodd"
								d="M5.22 14.78a.75.75 0 001.06 0l7.22-7.22v5.69a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75h-7.5a.75.75 0 000 1.5h5.69l-7.22 7.22a.75.75 0 000 1.06z"
								clip-rule="evenodd"
							></path>
						</svg></span
					></span
				></a
			>
		</div>
	</div>
</section>
