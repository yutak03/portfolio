<!-- src/components/Hero.svelte -->
<script>
    import { fade } from 'svelte/transition';
  </script>
  
  <section in:fade={{ duration: 2000 }}>
    <h1>Welcome to My Portfolio</h1>
    <p>Discover my work and projects.</p>
  </section>
  
  <style>
    section {
      text-align: center;
      padding: 5rem 1rem;
      background: #f0f0f0;
    }
  </style>
  