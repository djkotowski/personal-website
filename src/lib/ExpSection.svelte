<script>
  import Header from "./components/Header.svelte";
  import Link from "./components/Link.svelte";
</script>

<section class="container mx-auto text-center">
  <Header>Experience</Header>

  <ul
    class="mx-auto grid max-w-2xl grid-cols-1 gap-6 sm:grid-cols-2 lg:mx-0 lg:max-w-none lg:grid-cols-3 lg:gap-8"
  >
    <li class="rounded-2xl bg-gray-900 mx-2 px-8 py-10">
      <h2 class="text-2xl font-bold ">
        <Link href="https://brilliantmade.com/" target="_blank">Brilliant</Link>
      </h2>
      <div class="font-semibold mt-2 text-lg text-gray-300 ">
        <span class="block lg:inline-block">Software Engineer</span>
        <span class="block lg:inline-block">(Jul 2022 - Present)</span>
      </div>

      <hr class="border-gray-700 my-4" />

      <h5 class="font-semibold">Tech used:</h5>
      <p>Ruby on Rails, React, TypeScript, Alpine.js, MySQL, AWS, Redis, ActiveJob/Sidekiq</p>
    </li>
    <li class="rounded-2xl bg-gray-900 mx-2 px-8 py-10">
      <h2 class="text-2xl font-bold ">
        <Link href="https://buildout.com/" target="_blank">Buildout</Link>
      </h2>
      <ul class="font-semibold mt-2 text-lg text-gray-300 ">
        <li class="pb-2">
          <span class="block lg:inline-block">Lead Software Engineer</span>
          <span class="block lg:inline-block">(May 2021 - Jun 2022)</span>
        </li>
        <li class="pb-2">
          <span class="block lg:inline-block">Senior Software Engineer</span>
          <span class="block lg:inline-block">(Oct 2019 - May 2021)</span>
        </li>
        <li class="pb-2">
          <span class="block lg:inline-block">Software Engineer</span>
          <span class="block lg:inline-block">(May 2017 - Oct 2019)</span>
        </li>
      </ul>
      <hr class="border-gray-700 my-4" />

      <h5 class="font-semibold">Tech used:</h5>
      <p>Ruby on Rails, React, TypeScript, MySQL, AWS, Redis, Sidekiq</p>
    </li>
    <li class="rounded-2xl bg-gray-900 mx-2 px-8 py-10">
      <h2 class="text-2xl font-bold ">
        <Link href="https://cod.edu/" target="_blank">College of DuPage</Link>
      </h2>
      <div class="font-semibold mt-2 text-lg text-gray-300 ">
        <span class="block lg:inline-block">Adjunct Faculty</span>
        <span class="block lg:inline-block">(Aug 2014 - Dec 2017)</span>
      </div>

      <hr class="border-gray-700 my-4" />

      <h5 class="font-semibold">Courses taught:</h5>
      <p>CIS 1510: GUI Programming</p>
      <p>(using Visual Basic .NET)</p>
    </li>
    <li class="rounded-2xl bg-gray-900 mx-2 px-8 py-10">
      <h2 class="text-2xl font-bold ">
        <Link href="https://enova.com/" target="_blank">Enova International</Link>
      </h2>
      <ul class="font-semibold mt-2 text-lg text-gray-300 ">
        <li class="pb-2">
          <span class="block lg:inline-block">Internal Learning Coordinator</span>
          <span class="block lg:inline-block">(Dec 2014 - Mar 2017)</span>
        </li>
        <li class="pb-2">
          <span class="block lg:inline-block">Software Engineer</span>
          <span class="block lg:inline-block">(Aug 2014 - Dec 2014)</span>
        </li>
      </ul>

      <hr class="border-gray-700 my-4" />

      <h5 class="font-semibold">Tech used:</h5>
      <p>Ruby on Rails, Sinatra, Sidekiq</p>
    </li>
    <li class="rounded-2xl bg-gray-900 mx-2 px-8 py-10">
      <h2 class="text-2xl font-bold ">
        <Link
          href="https://www.accenture.com/us-en/services/supply-chain-management-and-operations-index"
          target="_blank"
        >
          Blue Horseshoe Solutions
        </Link>
        <br />
        <span class="block font-normal text-sm italic mt-0 pt-0">(now part of Accenture)</span>
      </h2>
      <div class="font-semibold mt-2 text-lg text-gray-300 ">
        <span class="inline-block">Consultant</span>
        <span class="inline-block">(May 2011 - Jan 2013)</span>
      </div>

      <hr class="border-gray-700 my-4" />

      <h5 class="font-semibold">Tech used:</h5>
      <p>C#, ASP.NET MVC 3, Microsoft SQL Server, jQuery, Manhattan SCALE</p>
    </li>
  </ul>
</section>
