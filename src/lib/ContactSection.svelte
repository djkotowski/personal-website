<script>
  import Header from "./components/Header.svelte";
  import GithubIcon from "./icons/GithubIcon.svelte";
  import Link from "./components/Link.svelte";
  import EnvelopeIcon from "./icons/EnvelopeIcon.svelte";
  import LinkedInIcon from "./icons/LinkedInIcon.svelte";
</script>

<section class="container mx-auto">
  <Header>Contact</Header>

  <div class="flex flex-row items-center justify-center space-x-12 lg:space-x-20">
    <div class="flex-initial">
      <Link href="mailto:dan@dankotowski.dev" target="_blank" title="Email me">
        <EnvelopeIcon class="w-12 h-12 lg:w-20 lg:h-20" />
        <div class="sr-only">Email me: dan@dankotowski.dev</div>
      </Link>
    </div>
    <div class="flex-initial">
      <Link href="https://github.com/djkotowski" target="_blank" title="Github">
        <GithubIcon class="w-12 h-12 lg:w-20 lg:h-20" />
        <div class="sr-only">Go to my Github account (@djkotowski)</div>
      </Link>
    </div>
    <div class="flex-initial">
      <Link href="https://linkedin.com/in/djkotowski" target="_blank" title="LinkedIn">
        <LinkedInIcon class="w-12 h-12 lg:w-20 lg:h-20" />
        <div class="sr-only">Go to my LinkedIn account (@djkotowski)</div>
      </Link>
    </div>
  </div>
</section>
