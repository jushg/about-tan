<script lang="ts">
  import { ArrowUpRight } from "lucide-svelte";

  import Seo from "$lib/components/Seo.svelte";

  const featuredProjects = [
    {
      name: "Cloud Jumpers",
      href: "/projects#cloudjumpers",
      desc: "iPadOS multiplayer platformer game",
      aside: "winner of the 20th NUS School of Computing Project Showcase",
    },
    {
      name: "Goose",
      href: "/projects#goose",
      desc: "a golang sublanguage interpreter written in Typescript",
      aside: "I learned how compilers, interpreters and golang work in the process",
    },
    {
      name: "Market Order Database",
      href: "/projects#marketdb",
      desc: "database for market orders time series data",
      aside: "proof of concept for a high performance time series database system",
    }
  ];
</script>

<Seo
  title="Hoang Trong Tan"
  description="Software engineer and tinkerer. Like to make new."
/>

<div class ="grid grid-cols-2 gap-4 layout-md pt-4">
  <p
    class="text-black text-xl leading-tight font-light mb-16"
    id="eric-is"
  >
    <span class="g">is a</span> programmer<span class="g">,</span><br />
    traveler<span class="g">, and</span><br />
    music enthusiast<span class="g">.</span>
  </p>
  <div class="gif flex items-center justify-center"> <img width="300" height="259" alt="RaccoonSpaceGif" src="/space.webp"> </div>
</div>

<div class="layout-md text-lg space-y-14">
  <div class="space-y-4">
    <p>
      I recently graduated with a Bachelor in Computer Engineering from the National University of Singapore.
    </p>

    <p>
      In my free time, I like to tinker with new ideas through personal projects, trying to learn random stuff in the process.
      I love C++, and have also touched on a lot of other interesting languages throughout my work experiences: Rust, Golang, Scala, Swift, Python, Typescript.
     </p>

     <p>
      I have interned at <a class="link" href="https://www.tiktok.com"
        >Tiktok</a>, <a class="link" href="https://www.polybee.co"
        >Polybee</a>, <a class="link" href="https://anduintransact.com/"
        >Anduin Transactions</a>, and most recently at <a class="link" href="https://parallelchain-lab.io"
        > ParallelChain Lab</a>
    </p>
  </div>
  <div class="leading-snug space-y-4">
    <p>Some notable projects that I think are cool:</p>
    {#each featuredProjects as project}
      <a class="project-pair bg-gray-100" href={project.href}>
        <div class="text-black font-medium">
          {project.name}
          <ArrowUpRight size={18} class="inline text-neutral-400" />
        </div>
        <div>
          <p>{project.desc}</p>
          {#if project.aside}
            <aside>{project.aside}</aside>
          {/if}
        </div>
      </a>
    {/each}
  </div>

  <div class="space-y-5">

  <p>I quite enjoy exploring different genres of music, and making random spotify playlists like this one:</p>

  <!-- svelte-ignore a11y-missing-attribute -->
  <iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/75ZeKv9AWkBvtGnplW3ZZT?utm_source=generator" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  </div>
</div>

<style lang="postcss">
  .g {
    @apply text-neutral-400;
  }

  em {
    @apply font-serif text-[110%] leading-[100%];
  }

  .project-pair {
    @apply grid sm:grid-cols-[1fr,2fr] gap-y-1 -mx-3 px-3 py-2 hover:bg-neutral-100 transition-colors;
  }

  aside {
    @apply mt-0.5 text-base text-neutral-500;
  }

  /* Correction for vertical navigation links on mobile. */
  @media (max-width: 420px) {
    #eric-is {
      @apply -mt-10;
    }
  }
</style>
