<script lang="ts">
  import { ArrowUpRight } from "lucide-svelte";

  import Seo from "$lib/components/Seo.svelte";

  const featuredProjects = [
    {
      name: "Cloud Jumpers",
      href: "/projects#cloudjumpers",
      desc: "iPadOS multiplayer platformer game",
      aside: "Winner of the 20th NUS School of Computing Project Showcase",
    },
    {
      name: "Peggle Redux",
      href: "/projects#peggle",
      desc: "a clone of the famous Peggle game",
      aside: "I built everything from scratch",
    },
  ];
</script>

<Seo
  title="Hoang Trong Tan"
  description="Software engineer, researcher, and designer. Making meaningful systems and interfaces for people."
/>

<p
  class="layout-md text-black text-xl leading-tight font-light mb-16"
  id="eric-is"
>
  <span class="g">is a</span> software engineer<span class="g">,</span><br />
  tinkerer<span class="g">, and</span><br />
  (amateur) competitive programmer<span class="g">.</span>
</p>

<div class="layout-md text-lg space-y-14">
  <div class="space-y-5">
    <p>
      I am currently a Computer Engineering undergraduate student at the National University of Singapore
    </p>

    <p>
      I am trying to learn more about algorithms and high-performance computing,and how they can address real-world problems. 
     </p> 

    <p>
     I usually tinker with new hardware and software through hackathons and personal projects, to try and make something cool. 
     Recently, I have also been fascinated by <em>Competitive Programming</em>, and have challenged myself with it. 
    </p>   
  </div>

  <div class="leading-snug space-y-4">
    <p class="pb-2">Some notable projects that I think is cool:</p>

    {#each featuredProjects as project}
      <a class="project-pair" href={project.href}>
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
    <p>
      I have worked at <a class="link" href="https://www.tiktok.com"
        >Tiktok</a
      >, <a class="link" href="https://www.polybee.co">Polybee</a>. 
    </p>

    <!-- <p>
      At NUS, I’ve been a distinguished teaching fellow for upper-level CS
      classes. I enjoy playing viola with various <a
        class="link"
        href="https://www.harvardradcliffeorchestra.org/">classical</a
      >
      <a class="link" href="https://youtu.be/rYrVFTzP4sw">music</a>
      <a class="link" href="https://youngarts.org/">groups</a>.
    </p> -->

    <p>Other interests: swimming, playing guitar, singing, and taking care of my cats.</p>
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
