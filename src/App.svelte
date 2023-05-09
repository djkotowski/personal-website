<script>
  import HeaderSection from "./lib/HeaderSection.svelte";
  import SkillsSection from "./lib/SkillsSection.svelte";
  import ExpSection from "./lib/ExpSection.svelte";
  import ContactSection from "./lib/ContactSection.svelte";
</script>

<div class="pb-16 lg:pb-24">
  <header class="bg-gray-900">
    <HeaderSection />
  </header>

  <main>
    <SkillsSection />
    <ExpSection />
    <ContactSection />
  </main>
</div>
