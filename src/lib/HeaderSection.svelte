<script>
import headshotPhoto from "../assets/headshot.jpg";
import Hero from "./components/Hero.svelte";
</script>

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
