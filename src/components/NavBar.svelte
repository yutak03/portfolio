<!-- src/components/NavBar.svelte -->
<script lang="ts">
    export let links = [];
    let siteName: string = "Yutak's Site";
  </script>
  
  <nav>
    <div class="container">
      <a href="/" class="logo">{siteName}</a>
      <ul>
        {#each links as link}
          <li><a href={link.href}>{link.text}</a></li>
        {/each}
      </ul>
    </div>
  </nav>
  
  <style>
    nav {
      background: linear-gradient(45deg, #007BFF, #FFD700);
      color: white;
      padding: 1rem 0;
    }
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 1rem;
    }
    .logo {
      font-size: 1.5rem;
      font-weight: bold;
      text-decoration: none;
      color: white;
    }
    ul {
      display: flex;
      list-style: none;
      padding: 0;
    }
    li {
      margin-right: 1rem;
    }
    a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }
    a:hover {
      color: #FFD700; /* Yellow on hover */
    }
  </style>
  