<script lang="ts">
  import Seo from "$lib/components/Seo.svelte";
  import Workplace from "./Workplace.svelte";
</script>

<Seo
  title="Trong Tan – Experiences"
  description="Software engineer and occasional spaghetti code creator."
/>

<section class="layout-md">

  <div class="gif flex items-center justify-center"> <img width="300" height="259" alt="RaccoonSpaceGif" src="/blog.webp"> </div>

  <h2>My most up-to-date resume is <a class="link" href="/resume_tan.pdf">here</a> </h2>

  <br/>

  <h2 class="heading2">Work Experiences</h2>

  <Workplace
  title="Blockchain Software Engineer Intern"
  company="ParallelChain Lab"
  url="https://parallelchain-lab.io"
  dates="April 2024 - Present"
  location="Singapore"
>
  <li>Worked on the Smart Contract SDK in the Layer 1 Blockchain Protocol team.</li>

</Workplace>

  <Workplace
  title="Fullstack Software Engineer Intern"
  company="Anduin Transactions"
  url="https://anduintransact.com/"
  dates="May 2023 - August 2023"
  location="Vietnam"
>
  <li>Managed development of a single-page web application for internal resources management, 
    used by a team of 50 engineers, built with Scala, FoundationDB and AWS.</li>
   <li> Implemented a lightweight embedded search engine using Apache Lucene's indexing and tokenization features.</li> 
   <li>Designed a fine-grained permission system for a privacy-sensitive internal data platform utilizing SpiceDB,
    a Google Zanzibar-inspired relationship-based access control model. </li>
</Workplace>

  <Workplace
    title="Backend Software Engineer Intern"
    company="Tiktok"
    url="https://tiktok.com/"
    dates="December 2022 - May 2023"
    location="Singapore"
  >
    <li>Developed REST endpoints for an e-Commerce data visualization website, use by internal business team and TiktokShop partners</li>
    <li>Designed a standardized paradigm utilizing Golang Generics for REST endpoints’ development of a backend service, removing 70% of redundant code in new features.</li>
    <li>Implemented an auto-testing script for QA to perform regression testing more easily on a data-intensive service, eliminating 95% of common regression bugs.</li>
  </Workplace>

  <Workplace
    title="Robotics Software Engineering Intern"
    company="Polybee"
    url="https://www.polybee.co"
    dates="May 2022 - August 2022"
    location="Singapore"
  >
    <li>Early-stage startup developing food solutions technology using micro-drones.</li>
    <li>Developed a micro-drone navigation algorithm based on V-SLAM research papers, and a mobile application for path planning, with a 90% success rate in flight operations.</li>
    <li>Led effort to create an in-house framework for drones navigation based on ROS2, migrating from TCP to UDP-based communication to remove single point of failure for the system.</li>
  </Workplace>


  <Workplace
    title="Research Assistant"
    company="NUS School of Design and Environment"
    url="https://cde.nus.edu.sg/dbe"
    dates="June 2021 – December 2021"
    location="Singapore"
  >
    <li>
      Prototyped a smart ventilation system using MQTT protocol, 
      Arduino and Raspberry Pi, with 40% increase in control accuracy and 30% of energy consumption reduction compared to previous system.
    </li>

  </Workplace>

</section>


<section class="layout-md py-4">
  <h2 class="heading2">Teaching Experiences</h2>

  <Workplace
    title="Undergraduate Teaching Assistant"
    company="NUS - School of Computing"
    url="https://www.comp.nus.edu.sg"
    dates="January 2022 – Present"
    location="Singapore"
  >
  <li>Grader, CS3217 (Software Engineering on Modern Application Platforms), Spring 2023 </li>
  <li>Lab Tutor, CS1010 (Programming Methodology), Fall 2022 and Spring 2022</li>
  <li>Project Advisor, CP2106 (Independent Software Development Project), Summer 2022 </li>
  <li>Lab Tutor, CS2040 (Data Structures and Algorithms), Spring 2022, Fall 2023, Spring 2024</li>
  </Workplace>
</section>

<section class="layout-md py-4">
  <h2 class="heading2">Education</h2>

  <Workplace
    title="B.Eng. in Computer Engineering"
    company="National University of Singapore"
    url="https://www.comp.nus.edu.sg"
    dates="August 2020 – May 2024"
    location="Singapore"
  >
  <li>Took a lot of CS modules, not enough EE modules </li>
  </Workplace>
</section>

<!-- <section class="layout-md pt-4">
  <h2 class="heading2">Awards and Honors</h2>

  <div class="mb-4">
    <ul>
      <li>
        <b> Ho Chi Minh University of Technology:</b> Entrance Valedictorian (2019)
      </li>
      <li>
        <b> 20th NUS School of Computing Project Showcase:</b> 1st Prize for CS3217 Project (Cloud Jumpers)
      </li>

    </ul>
  </div>
</section> -->

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
