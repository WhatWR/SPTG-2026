<svelte:head>
  <title>SPTG Nexus | Central Aviation Hub</title>
</svelte:head>

<div class="landing">
  <div class="header">
    <h1>Welcome to the SPTG Nexus</h1>
    <p class="subtitle">Your integrated hub for pilot knowledge, aerospace systems, and interactive exam mastery.</p>
  </div>

  <div class="card-grid">
    <a href="/aircraft" class="guide-card">
      <div class="emoji-icon">✈️</div>
      <h2>Aircraft Components</h2>
      <p>Visual study guide exploring aircraft anatomy, flight controls, and engine mechanics.</p>
    </a>
    
    <a href="/aviation" class="guide-card">
      <div class="emoji-icon">📘</div>
      <h2>Aviation Knowledge</h2>
      <p>Critical aviation theories, operations, and regulatory frameworks.</p>
    </a>
    
    <a href="/space" class="guide-card">
      <div class="emoji-icon">🚀</div>
      <h2>Space Science</h2>
      <p>Astrodynamics, atmospheric layers, and aerospace environment.</p>
    </a>
    
    <a href="/complete-guide" class="guide-card">
      <div class="emoji-icon">📚</div>
      <h2>Complete Study Guide</h2>
      <p>The ultimate 2026 comprehensive compendium of all aviation subjects.</p>
    </a>
    
    <a href="/quiz" class="guide-card quiz-card" style="grid-column: 1 / -1; max-width: 600px; justify-self: center;">
      <div class="emoji-icon">🎯</div>
      <h2>Quiz Master Pro</h2>
      <p>Test your synthesis of all subjects with the interactive simulator.</p>
    </a>
  </div>
</div>

<style>
  .landing {
    padding: 60px 32px;
    height: 100%;
    overflow-y: auto;
    background: radial-gradient(circle at center top, #0d1e38 0%, #060d1a 100%);
    box-sizing: border-box;
  }
  
  .header {
    text-align: center;
    margin-bottom: 56px;
  }

  h1 {
    font-size: 3rem;
    font-weight: 800;
    color: #fff;
    margin: 0 0 16px 0;
    text-shadow: 0 4px 20px rgba(66, 165, 245, 0.3);
  }

  .subtitle {
    color: #90caf9;
    font-size: 1.25rem;
    max-width: 600px;
    margin: 0 auto;
    line-height: 1.6;
  }

  .card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 28px;
    max-width: 1080px;
    margin: 0 auto;
  }

  .guide-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    background: rgba(13, 27, 46, 0.5);
    border: 1px solid rgba(66, 165, 245, 0.2);
    padding: 40px 24px;
    border-radius: 20px;
    text-decoration: none;
    color: inherit;
    transition: all 0.3s cubic-bezier(0.2, 0.8, 0.2, 1);
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
    backdrop-filter: blur(10px);
  }

  .guide-card:hover {
    transform: translateY(-8px);
    border-color: rgba(66, 165, 245, 0.6);
    box-shadow: 0 16px 40px rgba(66, 165, 245, 0.15);
    background: rgba(18, 38, 65, 0.7);
  }

  .emoji-icon {
    font-size: 3rem;
    margin-bottom: 20px;
    filter: drop-shadow(0 4px 8px rgba(0,0,0,0.4));
    transition: transform 0.3s ease;
  }

  .guide-card:hover .emoji-icon {
    transform: scale(1.15) translateY(-4px);
  }

  .guide-card h2 {
    font-size: 1.5rem;
    color: #e8eaf6;
    margin: 0 0 12px 0;
  }

  .guide-card p {
    color: #b0bec5;
    font-size: 0.95rem;
    margin: 0;
    line-height: 1.5;
  }

  .quiz-card {
    border-color: rgba(255, 204, 2, 0.3);
    background: linear-gradient(180deg, rgba(30, 25, 0, 0.6) 0%, rgba(13, 27, 46, 0.6) 100%);
  }
  
  .quiz-card:hover {
    border-color: rgba(255, 204, 2, 0.8);
    box-shadow: 0 16px 40px rgba(255, 204, 2, 0.15);
    background: linear-gradient(180deg, rgba(40, 32, 0, 0.7) 0%, rgba(18, 38, 65, 0.8) 100%);
  }
</style>
