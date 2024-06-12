<script>
    import { fade } from 'svelte/transition';
    import { onMount } from 'svelte';
  
    let showContent = false;
  
    onMount(() => {
      showContent = true;
    });
  </script>
  
  <section class="about">
    <div class="container" in:fade={{ duration: 1000 }}>
      <h1>Yutakについて</h1>
      <div class="profile">
        <div class="profile-info">
          <div class="profile-item">
            <strong>名前:</strong>
            <span>Yutak</span>
          </div>
          <div class="profile-item">
            <strong>生年月日:</strong>
            <span>1997年5月7日</span>
          </div>
        </div>
        <div class="social-links">
          <a href="https://github.com/yutak03" target="_blank" aria-label="GitHub">
            <img src="/img/github-mark.png" alt="GitHub" class="social-icon" />
          </a>
          <a href="https://x.com/yutak03" target="_blank" aria-label="Twitter">
            <img src="/img/x-mark.png" alt="X" class="social-icon" />
          </a>
        </div>
      </div>
      <div class="career">
        <h2>キャリア概要</h2>
        <p>
          Yutakはウェブ開発とソフトウェアエンジニアリングの強いバックグラウンドを持つ情熱的な開発者です。2019年にXYZ大学でコンピュータサイエンスの学位を取得しました。過去数年間で、Yutakは様々な企業と協力し、フロントエンドおよびバックエンドの開発において多くの成功したプロジェクトに貢献してきました。
        </p>
        <p>
          Yutakの専門分野には、React、Vue、Svelteなどの最新のJavaScriptフレームワーク、Node.jsやRustなどのバックエンド技術が含まれます。さらに、AWSを中心としたクラウドサービスにも精通しており、DevOpsの実践にも強い関心を持っています。
        </p>
        <p>
          技術的なスキルに加えて、Yutakは問題解決能力と継続的な学習への献身で知られています。テックコミュニティに積極的に参加し、ブログ投稿や公演を通じて知識を共有することを楽しんでいます。
        </p>
        <p>
          Yutakの卓越性へのコミットメントと協力的なアプローチは、どのチームにおいても貴重な資産となります。新しい課題に取り組む意欲があり、技術の進歩に貢献することを常に楽しみにしています。
        </p>
      </div>
      <div class="skills">
        <h2>スキル</h2>
        <ul>
          <li>AWS</li>
          <li>Java</li>
          <li>PHP</li>
          <li>Python</li>
          <li>Rust</li>
          <li>Svelte</li>
        </ul>
      </div>
    </div>
  </section>
  
  <style>
    .about {
      padding: 5rem 1rem;
      background: #f9f9f9;
      color: #333;
    }
    .container {
      max-width: 800px;
      margin: 0 auto;
      text-align: left;
    }
    h1, h2 {
      color: #007BFF;
    }
    .profile {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 2rem;
    }
    .profile-info {
      flex: 1;
    }
    .profile-item {
      margin-bottom: 1rem;
    }
    .profile-item strong {
      display: inline-block;
      width: 120px;
    }
    .social-links {
      display: flex;
      align-items: center;
    }
    .social-icon {
      width: 40px;
      height: 40px;
      margin-left: 1rem;
    }
    .career p {
      margin-bottom: 1rem;
      line-height: 1.6;
    }
    .skills {
      margin-top: 2rem;
    }
    .skills ul {
      list-style-type: none;
      padding: 0;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
    .skills li {
      background: #007BFF;
      color: white;
      display: inline-block;
      margin: 0.5rem;
      padding: 0.5rem 1rem;
      border-radius: 0.5rem;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .skills li:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
    }
  </style>
  