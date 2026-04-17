<script>
  let { children } = $props();
</script>

<div class="app-layout">
  <nav class="navbar">
    <div class="logo">✈️ SPTG Nexus</div>
    <ul class="nav-links">
      <li><a href="/">Home</a></li>
      <li><a href="/aircraft">Aircraft</a></li>
      <li><a href="/aviation">Aviation</a></li>
      <li><a href="/space">Space</a></li>
      <li><a href="/complete-guide">Complete Guide</a></li>
      <li><a href="/quiz" class="quiz-nav">Quiz Master</a></li>
    </ul>
  </nav>

  <main class="content-view">
    {@render children()}
  </main>
</div>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
    background: #060d1a;
    color: #e8eaf6;
    overflow: hidden; /* Hide outer scroll to let iframe scroll internally */
  }

  .app-layout {
    display: flex;
    flex-direction: column;
    height: 100vh;
    width: 100vw;
  }

  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 40px;
    height: 64px;
    background: rgba(10, 20, 35, 0.85);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border-bottom: 1px solid rgba(66, 165, 245, 0.2);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
    z-index: 100;
    flex-shrink: 0;
  }

  .logo {
    font-size: 1.3rem;
    font-weight: 800;
    color: #42a5f5;
    letter-spacing: 0.5px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .nav-links {
    list-style: none;
    display: flex;
    gap: 8px;
    margin: 0;
    padding: 0;
  }

  .nav-links a {
    text-decoration: none;
    color: #b0bec5;
    font-weight: 600;
    font-size: 0.9rem;
    transition: all 0.2s ease;
    padding: 10px 16px;
    border-radius: 8px;
  }

  .nav-links a:hover {
    color: #ffffff;
    background: rgba(66, 165, 245, 0.15);
  }

  .nav-links a.quiz-nav {
    color: #ffcc02;
    background: rgba(255, 204, 2, 0.1);
  }

  .nav-links a.quiz-nav:hover {
    background: rgba(255, 204, 2, 0.25);
    color: #fff;
  }

  .content-view {
    flex: 1;
    position: relative;
    width: 100%;
    height: calc(100vh - 64px); /* Fallback */
    overflow: hidden;
  }
</style>
