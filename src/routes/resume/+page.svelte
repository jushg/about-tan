<script lang="ts">
  import Seo from "$lib/components/Seo.svelte";
  import Workplace from "./Workplace.svelte";
</script>

<Seo
  title="Trong Tan – Resume"
  description="Software engineer, researcher, and designer. Making meaningful systems and interfaces for people."
/>

<section class="layout-md py-12">
  <h2 class="heading2">Education</h2>



  <div class="mb-4">
    <div class="flex justify-between items-end">
      <h3 class="text-black text-lg">National University of Singapore</h3>
      <div class="text-neutral-500 mb-0.5">2020 — Current</div>
    </div>
    <p class="byline">B.Eng in Computer Engineering</p>
  </div>

  <h4 class="font-medium mt-4 mb-1">Teaching:</h4>
  <ul>
    <li>
      TF for CS 153 (Compilers), Fall 2021 —
      <em>Certificate of Distinction in Teaching</em>
    </li>
    <li>
      TA for
      <a class="link" href="https://sgi.mit.edu/"
        >Summer Geometry Institute (SGI)</a
      >, Summer 2021
    </li>
    <li>
      TF for CS 161 (Operating Systems), Spring 2021 —
      <em>Certificate of Distinction in Teaching</em>
    </li>
    <li>TF for CS 182 (Artificial Intelligence), Fall 2020</li>
    <li>
      TF for CS 124 (Data Structures and Algorithms), Spring 2020 —
      <em>Commendation for Extraordinary Teaching</em>
    </li>
  </ul>


  <h4 class="font-medium mt-4 mb-1">Notable undergraduate technical coursework:</h4>
  <ul>
    <li>Compilers (CS 153)</li>
    <li>Operating Systems (CS 161)</li>
    <li>Computer Graphics (MIT 6.837)</li>
    <li>Nanotechnology Fabrication (MIT 6.2540)</li>
    <li>Chaotic Dynamical Systems (Math 118r)</li>
    <li>Number Fields (Math 129)</li>
    <li>Differential Topology (Math 132)</li>
    <li>Honors Abstract Algebra (Math 55a)</li>
    <li>Honors Real and Complex Analysis (Math 55b)</li>
  </ul>

</section>

<section class="layout-md py-12">
  <h2 class="heading2">Professional Experience</h2>

  <Workplace
    title="Software Engineer Intern"
    company="Tiktok"
    url="https://modal.com/"
    dates="December 2022 – Current"
    location="Singapore, Singapore"
  >
    <li>Backend Engineer for Data Intelligence team - global e-Commerce</li>
    <li>
      Working on low-latency distributed systems, a secure container runtime,
      and programming language & web interfaces.
    </li>
  </Workplace>

  <Workplace
    title="Software Engineering Intern"
    company="Prosper Robotics"
    url="https://prosper.org/"
    dates="January 2022"
    location="London, UK"
  >
    <li>
      Early-stage startup developing VR-teleoperated household robots. Worked
      with electrical and mechanical engineers.
    </li>
    <li>
      I wrote real-time (&lt;10 μs) embedded microcontrollers in C++, developed
      new network services and robot control systems in Go. Refactored a lot of
      code, fixed many bugs, ported software to a new robot, introduced
      continuous integration, tests, static type checking for Python.
    </li>
  </Workplace>


  <Workplace
    title="Software Engineering Intern"
    company="Scale AI"
    url="https://scale.com/"
    dates="December 2020 – January 2021"
    location="San Francisco, CA"
  >
    <li>
      Worked on machine learning infrastructure for a fast-growing startup using
      Terraform, Kubernetes, and AWS.
    </li>
    <li>
      Developed an in-house system to unify the ML training workflow, allowing
      the team to quickly iterate on models, share results on a tracking server,
      and launch Kubernetes distributed training jobs, saving “hours” of time on
      each experiment.
    </li>
  </Workplace>

  <Workplace
    title="Architecture Intern"
    company="Nvidia"
    url="https://www.nvidia.com"
    dates="June 2020 – August 2020"
    location="Santa Clara, CA"
  >
    <li>
      Worked with the Applied Deep Learning Research (ADLR) group on
      <a class="link" href="https://arxiv.org/abs/2005.10821"
        >deep learning models</a
      > for street image segmentation.
    </li>
    <li>
      Individually developed and released
      <a class="link" href="https://github.com/ekzhang/fastseg">FastSeg</a>, an
      open-source library containing state-of-the-art PyTorch implementations of
      MobileNetV3 LR-ASPP for real-time semantic segmentation, significantly
      more accurate than existing public implementations.
    </li>
  </Workplace>

  <Workplace
    title="Research Assistant"
    company="Harvard Programming Languages Group"
    url="https://pl.seas.harvard.edu/"
    dates="June 2020 – August 2020"
    location="Cambridge, MA"
    defaultHidden
  >
    <li>
      Worked on a C++ compiler for
      <a class="link" href="https://github.com/HarvardPL/formulog">Formulog</a>,
      a variant of Datalog that supports ML-like syntax extension and SMT
      queries.
    </li>
    <li>
      Generated highly parallel templatized C++17 code, used caching in B-Tree
      comparisons to speed up Datalog evaluation by 16x, and optimized existing
      OpenMP code using lockless data structures for an additional 4x speedup.
    </li>
    <li>
      Wrote a handwritten parser that was 30x faster than the ANTLR-generated
      LL(*) parser and used 20x less memory (80 GB to 4 GB).
    </li>
  </Workplace>

  <Workplace
    title="Undergraduate Researcher"
    company="Predictive Medicine Group"
    url="https://www.predmed.org/"
    dates="December 2019 – June 2020"
    location="Boston, MA"
    defaultHidden
  >
    <li>
      Conducted research in statistics & medical informatics advised by Ben Reis
      (Harvard Medical School), developing temporal models to identify patients
      at high risk of suicide based on medical histories obtained from
      Massachusetts General Hospital.
    </li>
  </Workplace>

</section>

<section class="layout-md py-12">
  <h2 class="heading2">Awards and Honors</h2>

  <div class="mb-4">
    <h3 class="font-medium mb-1">Computer Science:</h3>
    <ul>
      <li>
        <b>International Olympiad in Informatics (IOI):</b> Gold Medalist (2018,
        2019), 7<sup>th</sup> place globally
      </li>
      <li>
        <b>Google Hash Code:</b> World Finalist (2020, 2021, 2022), 6<sup
          >th</sup
        > place team out of over 100,000 students and professionals
      </li>
      <li>
        <b>Google Code Jam:</b> Round 3 Finalist (2020), placed 34<sup>th</sup>
        globally
      </li>
      <li><b>Facebook Hacker Cup:</b> Round 3 Finalist (2020)</li>
      <li><b>PicoCTF:</b> Winner (2018), ranked 6th</li>
    </ul>
  </div>

  <div class="mb-4">
    <h3 class="font-medium mb-1">Mathematics:</h3>
    <ul>
      <li>
        <b>Mathematical Olympiad Program (MOP):</b> Participant (2017), IMO team
        selection group (2017, 2018)
      </li>
      <li>
        <b>USA Math Olympiad (USAMO):</b> Honorable Mention (2017), top 24 in nation
      </li>
    </ul>
  </div>

  <div class="mb-4">
    <h3 class="font-medium mb-1">Physics:</h3>
    <ul>
      <li><b>U.S. Physics Team:</b> Invitee (2017, 2018, 2019)</li>
      <li>
        <b>USA Physics Olympiad (USAPhO):</b> Gold Medalist (2017, 2018, 2019)
      </li>
    </ul>
  </div>

  <div class="mb-4">
    <h3 class="font-medium mb-1">Music Performance:</h3>
    <ul>
      <li>
        <b>National YoungArts Foundation:</b> Winner in Classical Music (2018, 2019)
      </li>
      <li>
        <b>JDR Viola Competition:</b> Grand prize winner, performed with a professional
        orchestra (2019)
      </li>
      <li>
        <b>Texas All-State Symphony Orchestra:</b> Principal Violist (2017), Co-Principal
        (2016, 2018)
      </li>
    </ul>
  </div>
</section>

<style lang="postcss">
  b {
    @apply font-medium;
  }

  ul {
    @apply list-disc pl-7 marker:text-neutral-400;
  }

  .byline {
    @apply font-serif italic;
  }
</style>
