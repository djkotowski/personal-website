<script>
  import Header from "./components/Header.svelte";
</script>

<section class="container mx-auto px-4">
  <Header>Skills</Header>

  <div class="content-center lg:text-lg">
    <table class="mx-auto sm:whitespace-nowrap">
      <tr>
        <th class="block sm:table-cell font-bold w-auto pr-3 lg:pr-5 text-left">Backend:</th>
        <td class="block pb-4 sm:pb-0 sm:table-cell text-left">Ruby, Ruby on Rails, Node.js, Sinatra</td>
      </tr>
      <tr>
        <th class="block sm:table-cell font-bold w-auto pr-3 lg:pr-5 text-left">Frontend:</th>
        <td class="block pb-4 sm:pb-0 sm:table-cell text-left">ES6, TypeScript, React, Redux, Svelte, CSS/Sass, Webpack, Vite</td>
      </tr>
      <tr>
        <th class="block sm:table-cell font-bold w-auto pr-3 lg:pr-5 text-left">Data:</th>
        <td class="block pb-4 sm:pb-0 sm:table-cell text-left">PostgreSQL, MySQL, Redis, Elasticsearch</td>
      </tr>
    </table>
  </div>
</section>
