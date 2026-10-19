<script setup>
const projects = [
  { number: '01', name: 'A project worth sharing', description: 'A short note about what you made, who it helps, and what you learned along the way.', type: 'Selected project', href: 'https://github.com/tylerronning03' },
  { number: '02', name: 'Another good piece of work', description: 'Use this space for a side project, a collaboration, or something you are proud of.', type: 'In progress', href: 'https://github.com/tylerronning03' },
]
const year = new Date().getFullYear()
</script>

<template>
  <div class="min-h-screen overflow-hidden bg-[#f5f3ee] text-[#252922]">
    <header class="mx-auto flex w-full max-w-6xl items-center justify-between px-6 py-7 sm:px-10 lg:px-12">
      <a href="#top" class="flex items-center gap-3 text-sm font-semibold tracking-tight" aria-label="Tyler Ronning, home">
        <span class="grid size-9 place-items-center rounded-full bg-[#d8e2cf] font-serif text-lg">t.</span><span>Tyler Ronning</span>
      </a>
      <nav aria-label="Main navigation" class="flex items-center gap-5 text-sm text-[#62665d] sm:gap-8">
        <a class="transition hover:text-[#252922]" href="#about">About</a>
        <a class="transition hover:text-[#252922]" href="#work">Work</a>
        <a class="rounded-full border border-[#c9cbc2] px-4 py-2 text-[#252922] transition hover:border-[#252922]" href="mailto:hello@example.com">Say hello <span aria-hidden="true">↗</span></a>
      </nav>
    </header>

    <main id="top" class="mx-auto w-full max-w-6xl px-6 sm:px-10 lg:px-12">
      <section class="relative grid min-h-[590px] items-center py-16 sm:py-20 lg:grid-cols-[1.2fr_0.8fr] lg:py-24">
        <div class="pointer-events-none absolute -right-36 top-10 -z-0 size-[28rem] rounded-full bg-[#e2e8d9] opacity-70 blur-3xl" aria-hidden="true"></div>
        <div class="relative z-10 max-w-3xl">
          <p class="mb-8 flex items-center gap-3 text-xs font-semibold uppercase tracking-[0.22em] text-[#72776b]"><span class="size-2 rounded-full bg-[#77916b]"></span>Personal site · <span>{{ year }}</span></p>
          <h1 class="max-w-3xl font-serif text-6xl leading-[0.98] tracking-[-0.055em] sm:text-7xl lg:text-[6.5rem]">Making useful things <span class="italic text-[#718666]">for people.</span></h1>
          <p class="mt-8 max-w-xl text-lg leading-8 text-[#62665d] sm:text-xl">I’m Tyler, a curious builder who enjoys turning thoughtful ideas into clear, useful experiences on the web.</p>
          <div class="mt-10 flex flex-wrap items-center gap-4">
            <a href="#work" class="inline-flex items-center gap-3 rounded-full bg-[#252922] px-6 py-3.5 text-sm font-medium text-white transition hover:bg-[#42483d]">Explore my work <span aria-hidden="true">↓</span></a>
            <a href="https://github.com/tylerronning03" class="inline-flex items-center gap-2 px-3 py-3 text-sm font-medium text-[#454a41] transition hover:text-[#718666]">Find me on GitHub <span aria-hidden="true">↗</span></a>
          </div>
        </div>
        <div class="relative z-10 mt-14 lg:mt-0 lg:justify-self-end">
          <div class="relative aspect-[4/5] w-full max-w-[340px] overflow-hidden rounded-[11rem_11rem_1.25rem_1.25rem] bg-[#dce4d4] p-5 sm:max-w-[390px]">
            <div class="absolute inset-5 overflow-hidden rounded-[10rem_10rem_0.75rem_0.75rem] border border-white/50 bg-[#cbd8c2]">
              <div class="absolute inset-0 bg-[radial-gradient(ellipse_at_50%_38%,rgba(255,255,255,.8),transparent_46%),linear-gradient(145deg,#dce5d5_10%,#b9c9af_68%,#a4b79a)]"></div>
              <div class="absolute bottom-0 left-1/2 h-[57%] w-[75%] -translate-x-1/2 rounded-t-[48%] bg-[#8e9f83]"></div>
              <div class="absolute bottom-[32%] left-1/2 h-[36%] w-[34%] -translate-x-1/2 rounded-[48%] bg-[#e8c9aa]"></div>
              <div class="absolute bottom-[55%] left-1/2 h-[14%] w-[37%] -translate-x-1/2 rounded-t-full bg-[#42483d]"></div>
              <span class="absolute bottom-5 left-0 right-0 text-center font-serif text-sm italic text-[#4d5b47]">A little space to make things</span>
            </div>
            <span class="absolute bottom-7 right-7 grid size-12 place-items-center rounded-full bg-[#f5f3ee] font-serif text-xl text-[#718666]" aria-hidden="true">✳</span>
          </div>
        </div>
      </section>

      <section id="about" class="grid gap-8 border-t border-[#d9d9d1] py-16 sm:py-20 lg:grid-cols-[0.7fr_1.3fr] lg:gap-16">
        <div><p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#85897f]">A bit about me</p><h2 class="mt-4 font-serif text-3xl tracking-tight sm:text-4xl">Curiosity, with a purpose.</h2></div>
        <div class="max-w-2xl space-y-5 text-base leading-7 text-[#62665d] sm:text-lg sm:leading-8">
          <p>This is my corner of the internet: a home for the projects I care about, ideas I’m exploring, and the people I meet along the way.</p>
          <p>I like working across the whole process, from the first sketch to the details that make a finished product feel considered. I’m currently interested in <span class="text-[#343a31]">good design, useful technology, and learning in public.</span></p>
        </div>
      </section>

      <section id="work" class="border-t border-[#d9d9d1] py-16 sm:py-20">
        <div class="mb-10 flex flex-wrap items-end justify-between gap-4"><div><p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#85897f]">A few highlights</p><h2 class="mt-4 font-serif text-3xl tracking-tight sm:text-4xl">Selected work</h2></div><a class="text-sm font-medium text-[#62665d] transition hover:text-[#252922]" href="https://github.com/tylerronning03">More on GitHub <span aria-hidden="true">↗</span></a></div>
        <div class="grid gap-4 md:grid-cols-2">
          <a v-for="project in projects" :key="project.number" :href="project.href" class="group rounded-3xl border border-[#d9d9d1] bg-white/40 p-6 transition hover:-translate-y-1 hover:border-[#bfc7b8] hover:bg-white/70 sm:p-8">
            <div class="flex items-center justify-between text-xs font-medium uppercase tracking-[0.16em] text-[#85897f]"><span>{{ project.type }}</span><span>{{ project.number }}</span></div>
            <div class="mt-14 flex items-start justify-between gap-4"><div><h3 class="font-serif text-2xl tracking-tight">{{ project.name }}</h3><p class="mt-3 max-w-md text-sm leading-6 text-[#70746b]">{{ project.description }}</p></div><span class="mt-1 text-xl text-[#718666] transition group-hover:translate-x-1 group-hover:-translate-y-1" aria-hidden="true">↗</span></div>
          </a>
        </div>
      </section>

      <section class="mb-16 rounded-[2rem] bg-[#dce4d4] px-7 py-10 sm:mb-20 sm:px-12 sm:py-14">
        <div class="flex flex-col justify-between gap-8 sm:flex-row sm:items-end"><div><p class="text-xs font-semibold uppercase tracking-[0.22em] text-[#66765e]">Have something in mind?</p><h2 class="mt-4 max-w-xl font-serif text-4xl leading-tight tracking-tight sm:text-5xl">Let’s make a good thing happen.</h2></div><a href="mailto:hello@example.com" class="inline-flex w-fit items-center gap-3 rounded-full bg-[#252922] px-6 py-3.5 text-sm font-medium text-white transition hover:bg-[#42483d]">Get in touch <span aria-hidden="true">↗</span></a></div>
      </section>
    </main>

    <footer class="mx-auto flex w-full max-w-6xl flex-col gap-4 border-t border-[#d9d9d1] px-6 py-7 text-xs text-[#85897f] sm:flex-row sm:items-center sm:justify-between sm:px-10 lg:px-12">
      <span>© {{ year }} Tyler Ronning. Made with care.</span><div class="flex gap-5"><a class="transition hover:text-[#252922]" href="https://github.com/tylerronning03">GitHub ↗</a><a class="transition hover:text-[#252922]" href="mailto:hello@example.com">Email ↗</a></div>
    </footer>
  </div>
</template>
