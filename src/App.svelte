<script>
  let accordionItems = [
    { title: 'What is Stylescape?', content: 'Stylescape is a comprehensive CSS framework designed to streamline web development with modern design patterns and utilities.' },
    { title: 'How to use it?', content: 'Simply import Stylescape into your project and start using the pre-built components and utility classes.' },
    { title: 'Is it customizable?', content: 'Yes! Stylescape is built with SCSS and provides extensive customization options through variables and mixins.' }
  ];
</script>

<div class="frame_main">
  <!-- Top Ribbon / Header -->
  <header class="ribbon--top">
    <div class="container">
      <h1>Stylescape Svelte Example</h1>
      <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
      <button data-ss="theme-toggle" aria-label="Toggle theme">
        🌓 Toggle Theme
      </button>
    </div>
  </header>

  <!-- Left Sidebar -->
  <aside class="sidebar--left" data-ss="aside">
    <nav>
      <h3>Navigation</h3>
      <ul>
        <li><a href="#dashboard">Dashboard</a></li>
        <li><a href="#settings">Settings</a></li>
        <li><a href="#profile">Profile</a></li>
      </ul>
    </nav>
  </aside>

  <!-- Main Content -->
  <main class="content">
    <section class="container">
      <h2>Welcome to Stylescape</h2>
      <p>This is a demonstration of Stylescape integration with Svelte and Vite.</p>

      <!-- Accordion Component -->
      <div class="accordion" data-ss="accordion">
        {#each accordionItems as item, index}
          <div class="accordion__item">
            <button class="accordion__header" aria-expanded="false">
              {item.title}
            </button>
            <div class="accordion__content">
              <p>{item.content}</p>
            </div>
          </div>
        {/each}
      </div>

      <!-- Sample Buttons -->
      <div class="button-group" style="margin-top: 2rem;">
        <button class="btn btn--primary">Primary Button</button>
        <button class="btn btn--secondary">Secondary Button</button>
        <button class="btn btn--outline">Outline Button</button>
      </div>
    </section>
  </main>

  <!-- Right Sidebar -->
  <aside class="sidebar--right" data-ss="aside">
    <div>
      <h3>Info Panel</h3>
      <p>Additional content and widgets can be placed here.</p>
    </div>
  </aside>

  <!-- Bottom Ribbon / Footer -->
  <footer class="ribbon--bottom">
    <div class="container">
      <p>&copy; 2026 Stylescape. All rights reserved.</p>
    </div>
  </footer>
</div>

<style>
  /* Component-specific styles can be added here */
  .container {
    padding: 1rem;
  }

  header .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1rem;
  }

  header nav {
    display: flex;
    gap: 1rem;
  }

  header nav a {
    text-decoration: none;
  }

  .button-group {
    display: flex;
    gap: 0.5rem;
    flex-wrap: wrap;
  }
</style>
