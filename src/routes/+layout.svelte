<!-- src/routes/+layout.svelte -->
<script>
    import NavBar from '../components/NavBar.svelte';
    import Footer from '../components/Footer.svelte';
  
    const links = [
      { href: '/', text: 'Home' },
      { href: '/about', text: 'About' },
      { href: '/projects', text: 'Projects' },
      { href: '/contact', text: 'Contact' },
    ];
  </script>
  
  <NavBar {links} />
  
  <main>
    <slot />
  </main>
  
  <Footer />
  
  <style>
    main {
      padding: 2rem;
    }
  </style>
  