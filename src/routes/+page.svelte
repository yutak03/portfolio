<script>
    import { fade } from 'svelte/transition';
    import { onMount } from 'svelte';
  
    let showContent = false;
  
    onMount(() => {
      showContent = true;
    });
  </script>
  
  <section class="hero">
    <div class="container">
      {#if showContent}
        <h1 in:fade={{ duration: 1000 }}>ようこそ、私のポートフォリオへ</h1>
        <p in:fade={{ duration: 1500 }}>作品やプロジェクトをぜひご覧ください。</p>
        <a href="/projects" class="btn" in:fade={{ duration: 2000 }}>プロジェクトを見る</a>
      {/if}
    </div>
  </section>
  
  <section class="about">
    <div class="container">
      <h2>私について</h2>
      <p>
        私はウェブ開発が大好きなエンジニアです。美しくて使いやすいウェブアプリケーションを作るのが得意です。
        私の経歴やスキルについてもっと知りたい方は、以下をチェックしてください！
      </p>
      <a href="/about" class="btn">もっと知る</a>
    </div>
  </section>
  
  <style>
    .hero {
      background: linear-gradient(45deg, #007BFF, #FFD700);
      color: white;
      padding: 5rem 1rem;
      text-align: center;
    }
    .hero .container {
      max-width: 1200px;
      margin: 0 auto;
    }
    .hero h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }
    .hero p {
      font-size: 1.25rem;
      margin-bottom: 2rem;
    }
    .hero .btn {
      background: white;
      color: #007BFF;
      padding: 0.75rem 1.5rem;
      border-radius: 0.5rem;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s ease, color 0.3s ease;
    }
    .hero .btn:hover {
      background: #007BFF;
      color: white;
    }
    
    .about {
      background: #f9f9f9;
      color: #333;
      padding: 5rem 1rem;
      text-align: center;
    }
    .about .container {
      max-width: 1200px;
      margin: 0 auto;
    }
    .about h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }
    .about p {
      font-size: 1.25rem;
      margin-bottom: 2rem;
    }
    .about .btn {
      background: #007BFF;
      color: white;
      padding: 0.75rem 1.5rem;
      border-radius: 0.5rem;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s ease, color 0.3s ease;
    }
    .about .btn:hover {
      background: #0056b3;
    }
  </style>
  