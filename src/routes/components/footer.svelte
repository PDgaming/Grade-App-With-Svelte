<script>
  import companyLogo from "../images/company-logo.png"; //imports logo image from images
</script>

<footer class="footer bg-base-200 text-base-content p-10">
  <aside>
    <a href="https://pd-enterprise.pages.dev" class="link link-hover">
      <img src={companyLogo} alt="logo" id="footer-logo" />
      <p>
        PD Enterprise
        <br />
        Providing reliable tech tools for students since 2024
      </p>
    </a>
  </aside>
  <nav>
    <h6 class="footer-title">Services</h6>
    <a href="https://grade-app.pages.dev" class="link link-hover">Grade App</a>
    <a href="https://cnotes.pages.dev" class="link link-hover">Cnotes</a>
  </nav>
  <nav>
    <h6 class="footer-title">Company</h6>
    <a href="https://pd-enterprise.pages.dev/about-us" class="link link-hover"
      >About us</a
    >
    <a href="https://pd-enterprise.pages.dev/contact" class="link link-hover"
      >Contact</a
    >
  </nav>
  <nav>
    <h6 class="footer-title">Social</h6>
    <div class="grid grid-flow-col gap-4">
      <a href="https://x.com/pd-enterprise">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          class="fill-current"
        >
          <path
            d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"
          ></path>
        </svg>
      </a>
      <a href="https://www.youtube.com/">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          class="fill-current"
        >
          <path
            d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"
          ></path>
        </svg>
      </a>
    </div>
  </nav>
</footer>

<style>
  :root {
    --image-size: 80px;
  }
  #footer-logo {
    width: var(--image-size);
    border-radius: 100px;
    cursor: pointer;
    margin-bottom: 10px;
    filter: brightness(0) invert(1);
  }
</style>
