<script lang="ts">
	import TimelineEntryCard from '$lib/components/ui/timeline-entry-card/timeline-entry-card.svelte';
	import resume from '$lib/assests/ResumeRyanPalmer.pdf';
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
					description="Designed and implemented a scalable distributed backend composed of AWS SAM lambda functions and a Kotlin rest api that served and handled requests for thousands of gig workers online banking needs, background checks, and tax services. 
					Improved customer acquisition in the onboarding process from 40% to 73% via a simplified signup workflow. Leading to quicker signups, preapprovals, and easier background checks.
					Created automated syncs for customer support to load customer data from Levels system into Zendesk that would seamlessly come up when a customer called in."
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
					description="Lead a team of engineers to build out a phone integration for Webex expanding Tenfold's customer support system platform. Driving the acquisition of new business that are using modern online phone systems.
					Developed a live call transcribing integration that would log live speech to text of calls into support tickets in sales force."
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
					description="Improved app performance and development cycles by migrating and modernizing web chat app from Angular.js to Angular 13 in 6 months, using a duplicate app and iterative approach.
					Utilized Cypress for end-to-end testing, achieving 70% code coverage and improving user experience, resulting in increased customer satisfaction and application stability.
					Lead development of Android app, adding new features & keeping it in sync with IOS & web."
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
					description="Worked as a part of a team of developers creating and updating python web applications for a consulting firm. Completing all work within strict timeframes and budgets maintaining product quality by keeping at least 90% automated tests coverage.
					Redeapp was one of the clients and they hired me to be part of their team because of the 3 months of work I had done for them."
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
					description="Created and maintained containerized Node.js integrations and libraries for Astronomers open sourced Analytics.js Platform.
					Designed Airflow data pipelines written in Node.js and python connecting external data sources to databases sending up to millions of events with test coverage in Mocha, Chai, and Nock."
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
