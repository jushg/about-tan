<script lang="ts">
  import Seo from "$lib/components/Seo.svelte";
  import Workplace from "./Workplace.svelte";
</script>

<Seo
  title="Trong Tan – Resume"
  description="Software engineer and occasional spagehetti code creator."
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
      Grader for CS3217 (Software Engineering on Modern Application Platforms), Spring 2023 
    </li>
    <li>
      Tutor for CS1010 (Programming Methodology) and CS2040 (Data Structures and Algorithms), Fall 2022
    </li>
    <li>
      Advisor for CP2106 (Independent Software Development Project), Summer 2022 
    </li>
    <li> Tutor for CS1010 (Programming Methodology), Spring 2022</li>
  </ul>


  <h4 class="font-medium mt-4 mb-1">Notable undergraduate technical coursework:</h4>
  <ul>
    <li>Competitive Programming (CS3233)</li>
    <li>Software Engineering on Modern Application Platforms (CS3217)</li>
    <li>Software Product Engineering for Digital Markets (CS3216)</li>
  </ul>

</section>

<section class="layout-md py-12">
  <h2 class="heading2">Professional Experience</h2>

  <Workplace
  title="Software Engineer Intern"
  company="Anduin Transactions"
  url="https://anduintransact.com/"
  dates="May 2023 - Current"
  location="Vietnam"
>
  <li>Developed the internal IDE used by other developer to build smart legal contract.</li>
</Workplace>

  <Workplace
    title="Software Engineer Intern"
    company="Tiktok"
    url="https://tiktok.com/"
    dates="December 2022 - May 2023"
    location="Singapore"
  >
    <li>Developed REST endpoints for an e-Commerce merchant data service website to integrate and visualize data from SQL database and other RPC endpoints.</li>
    <li>Setup an asynchronous export-to-excel service using ByteDance cloud function.</li>
  </Workplace>

  <Workplace
    title="Software Engineering Intern"
    company="Polybee"
    url="https://www.polybee.co"
    dates="May 2022 - August 2022"
    location="Singapore"
  >
    <li>
      Early-stage startup developing food solutions technology using micro-drones. Joined
      the micro-drone navigation and control developement team.
    </li>
    <li>
      Developed a micro-drone navigation pipeline with Visual-SLAM algorithms, with 90% success rate in operations and 80% increase in possible flight-duration.
    </li>
    <li>Led the effort to create an in-house framework for drones' automatic navigation using ROS2, pivoting from TCP to UDP-based communication.</li>
  </Workplace>


  <Workplace
    title="Research Assistant"
    company="NUS School of Design and Environment"
    url="https://cde.nus.edu.sg/dbe"
    dates="June 2021 – December 2021"
    location="Singapore"
  >
    <li>
      Designed and implemented an improved prototype of a smart ventilation system using MQTT protocol, Arduino and Raspberry  Pi, with 40% increase in response accuracy and 30% of power saved.
    </li>

  </Workplace>

</section>

<section class="layout-md py-12">
  <h2 class="heading2">Awards and Honors</h2>

  <div class="mb-4">
    <h3 class="font-medium mb-1">Computer Science:</h3>
    <ul>
      <li>
        <b>NUS STEPS 20th:</b> 1st Prize for CS3217 Project Showcase
      </li>

    </ul>
  </div>

    <!-- <h3 class="font-medium mb-1">Music Performance:</h3>
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
    </ul> -->
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
