<section
id="about"
class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24"
aria-label="About me"
>
<div
  class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
>
  <h2 class="text-sm font-bold uppercase tracking-widest text-slate-200 lg:sr-only">
    About
  </h2>
</div>
<div>
  <p class="mb-4">
    The first Hello World I ever wrote was in a 9th grade elective class in <a
    class="font-medium text-slate-200 hover:text-teal-300 focus-visible:text-teal-300"
    href="https://en.wikipedia.org/wiki/Racket_(programming_language)"
    target="_blank"
    rel="noreferrer noopener"
    aria-label="Racket programming_language (opens in a new tab)"
    >Racket</a>. This led to taking 3 more classes learning the fundamentals of loops, variables, code testing, and making 8 bit video games. Since then I've had the privilege of building out software for an insurance company, 4 start ups, and a lot of interesting projects in between.  
  </p>

  <p class="mb-4">
    Currently seeking an engaging fullstack or frontend role using a more modern stack using these prefered Languages, Frameworks, DBs: <br> 
  </p>
  <ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
    {#each ['React', 'Svelte', 'Next.js', 'Flutter', 'Python', 'Kotlin', 'Postgres', 'MongoDB', 'MySql', 'SQLite'] as tech}
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
</section>