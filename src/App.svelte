<script>
  import Hero from './lib/components/Hero.svelte'
  import headshotPhoto from './assets/headshot.jpg'
  import SkillsSection from "./lib/SkillsSection.svelte";
  import ExpSection from "./lib/ExpSection.svelte";
  import ContactSection from "./lib/ContactSection.svelte";
</script>

<div class="pb-16 lg:pb-24">
  <header class="bg-gray-900">
    <div class="container mx-auto">
      <Hero
        imageUrl={headshotPhoto}
        imageAlt="Headshot photograph of Dan Kotowski"
        title="Dan Kotowski"
      >
        <p class="mt-6 text-lg lg:text-xl text-gray-300">
          Senior web software engineer with strong technical and interpersonal skills
        </p>
        <p class="mt-6 text-yellow-600 italic">
          Note: This webpage is a work in progress.
        </p>
      </Hero>
    </div>
  </header>

  <main>
    <SkillsSection />
    <ExpSection />
    <ContactSection />
  </main>
</div>
