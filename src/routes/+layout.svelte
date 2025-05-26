<script lang="ts">
  import { onMount } from 'svelte';
  import { page } from '$app/stores';
  import { derived } from 'svelte/store';

  const path = derived(page, ($page) => $page.url.pathname);

  onMount(() => {
    path.subscribe(($path) => {
      if ($path === '/') {
        document.title = 'LEE HOKYUNG';
      } else if ($path.startsWith('/works')) {
        document.title = 'WORKS | LEE HOKYUNG';
      } else if ($path.startsWith('/exhibition')) {
        document.title = 'EXHIBITION | LEE HOKYUNG';
      } else if ($path.startsWith('/cv')) {
        document.title = 'CV | LEE HOKYUNG';
      }
    });
  });
</script>

<div class="main">
  <section class="header">
    <a href="/" class="home">이호경<br/>LEE HOKYUNG</a>
    <div class="nav-container">
      <nav class="main">
        <a href="/">HOME</a>
        <a href="/works/2020">WORKS</a>
        <a href="/exhibition">EXHIBITION</a>
        <a href="/cv">CV</a>
        <a href="https://www.instagram.com/art_work.hokka" target="_blank  "
          ><img src="/insta.png" alt="" width="30" height="30" /></a
        >
      </nav>
      <nav class="work-container">
        {#if $path.startsWith('/works')}
          <a href="/works/2020" class={$path === '/works/2020' ? 'on' : ''}
            >2020.</a
          >
          <a href="/works/2021" class={$path === '/works/2021' ? 'on' : ''}
            >2021.</a
          >
          <a href="/works/2023" class={$path === '/works/2023' ? 'on' : ''}
            >2023.</a
          >
        {/if}
      </nav>
    </div>
  </section>
  <slot />
</div>

<style>
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
    margin-left: 40px;
    margin-right: 40px;
    margin-bottom: 40px;
  }
  .home {
    font-size: 2rem;
    font-weight: 700;
    color: #000;
    text-decoration: none;
  }
  .header .main {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 600px;
  }
  .header .main a {
    font-size: 1.2rem;
    font-weight: 700;
    color: #000;
    text-decoration: none;
  }
  .nav-container {
    display: flex;
    flex-direction: column;
    margin-top: 30px;
  }
  .work-container {
    display: flex;
    width: 50%;
    justify-content: space-between;
    margin-top: 10px;
    margin-left: 100px;
    height: 30px;
  }
  .work-container a {
    font-size: 15px;
    font-weight: 700;
    color: #000;
    text-decoration: none;
  }
  .work-container .on {
    color: #000;
    border-bottom: 1px solid #000;
  }
  :global(figure) {
    display: block;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 10px;
    margin-inline-end: 10px;
  }
  @font-face {
    font-family: 'Noto Sans KR';
    src: url('/fonts/NotoSansCJKkr-Regular.otf');
  }
  :global(body) {
    font-size: 15px;
    font-family: 'Noto Sans KR', sans-serif;
  }
  .main {
    margin: auto;
    width: 1440px;
  }
</style>
