<!-- src/components/Footer.svelte -->
<script lang="ts">
    let currentYear: number = new Date().getFullYear();
    let name: string = "Yutak";
</script>

<footer>
    <div class="container">
      <p>&copy; {currentYear} {name}.</p>
      <nav>
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/about">About</a></li>
          <li><a href="/projects">Projects</a></li>
          <li><a href="/contact">Contact</a></li>
        </ul>
      </nav>
    </div>
  </footer>
  
  <style>
    footer {
      background: linear-gradient(45deg, #007BFF, #FFD700);
      color: white;
      padding: 2rem 0;
    }
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 1rem;
    }
    nav ul {
      display: flex;
      list-style: none;
      padding: 0;
    }
    nav li {
      margin-right: 1rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #FFD700; /* Yellow on hover */
    }
    p {
      margin: 0;
      font-size: 0.9rem;
    }
  </style>
  