<script lang="ts">
  function smoothScroll(event: Event) {
    event.preventDefault();
    const target = (event.target as HTMLAnchorElement).getAttribute("href");
    if (target && target.startsWith("#")) {
      const element = document.querySelector(target);
      if (element) {
        element.scrollIntoView({ behavior: "smooth" });
      }
    }
  }
</script>

<div class="navbar bg-base-200">
  <div class="navbar-start">
    <div class="dropdown">
      <div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h8m-8 6h16"
          />
        </svg>
      </div>
      <ul
        class="menu menu-sm dropdown-content bg-base-100 rounded-box z-[1] mt-3 p-2 shadow"
      >
        <li><a href="#home" on:click={smoothScroll}>Home</a></li>
        <li>
          <a href="#features" on:click={smoothScroll}>Features</a>
        </li>
        <li>
          <a href="#usage" on:click={smoothScroll}>Usage</a>
        </li>
        <li>
          <a href="#acknowledgments" on:click={smoothScroll}>Acknowledgments</a>
        </li>
        <li>
          <a href="#contact" on:click={smoothScroll}>Contact</a>
        </li>
        <li><a class="btn" href="/login">Login</a></li>
      </ul>
    </div>
    <a href="/" class="btn btn-ghost text-3xl">Grade App</a>
  </div>
  <div class="navbar-center hidden lg:flex">
    <ul class="menu menu-horizontal text-xl">
      <li><a href="#home">Home</a></li>
      <li>
        <a href="#features">Features</a>
      </li>
      <li>
        <a href="#usage">Usage</a>
      </li>
      <li>
        <a href="#acknowledgments">Acknowledgments</a>
      </li>
      <li>
        <a href="#contact">Contact</a>
      </li>
      <li><a href="/login" class="text-xl">Login</a></li>
    </ul>
  </div>
</div>

<style>
  .navbar {
    position: sticky;
    top: 0;
    z-index: 10;
    background-color: var(--base-100);
    backdrop-filter: blur(20px);
  }
</style>
