<script lang="ts">
  import "./styles.css"; //imports styles.css file
  import { registerServiceWorker } from "../registerServiceWorker"; //imports registerService Worker function from registerServiceWorker to register the service worker
  import "../app.css"; //imports app.css file for tailwindcss support

  registerServiceWorker(); //registers the service worker
</script>

<div class="app">
  <main>
    <slot></slot>
  </main>
</div>

<style>
</style>
