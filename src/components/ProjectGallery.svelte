<!-- src/components/ProjectGallery.svelte -->
<script>
    export let projects = [];
  </script>
  
  <section>
    {#each projects as project}
      <div class="project">
        <img src={project.image} alt={project.title} />
        <h3>{project.title}</h3>
        <p>{project.description}</p>
      </div>
    {/each}
  </section>
  
  <style>
    section {
      display: flex;
      flex-wrap: wrap;
    }
    .project {
      margin: 1rem;
      padding: 1rem;
      border: 1px solid #ccc;
      border-radius: 8px;
      width: calc(33.333% - 2rem);
    }
    img {
      max-width: 100%;
      border-radius: 8px;
    }
  </style>
  