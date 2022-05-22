<template>
  <footer class="bg-secondary text-primary-text-light mt-5">
    <div class="container py-5 border-bottom">
      <div class="row">
        <div class="col-3 title">
          <h3>JC DESIGN</h3>
        </div>
        <div class="col-3 nav-1">
          <div class="menu h5 fw-bold mb-3">Menu</div>
          <ul class="p-0">
            <li>About</li>
            <li>Services</li>
            <li>Blog</li>
            <li>Contact</li>
          </ul>
        </div>
        <div class="col-3 nav-2">
          <div class="menu h5 fw-bold mb-3">Service</div>
          <ul class="p-0">
            <li>Design</li>
            <li>Development</li>
            <li>Marketing</li>
            <li>See more</li>
          </ul>
        </div>
        <div class="col-3 external-links d-flex gap-4">
          <i class="bi bi-facebook text-primary" style="font-size: 1.5rem"></i>
          <i class="bi bi-linkedin text-primary" style="font-size: 1.5rem"></i>
          <i class="bi bi-twitter text-primary" style="font-size: 1.5rem"></i>
        </div>
      </div>
    </div>
    <div class="container py-5 d-flex justify-content-between">
      <div class="copyright">
        <p>Copyright © 2022 Laaqiq. All Rights Reserved.</p>
      </div>
      <div class="termsofuse-privacy d-flex gap-4">
        <p>Terms Of Use</p>
        <p>Privacy Policy</p>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  min-height: 50vh;
  width: 100%;
  border-radius: 10px 10px 0 0;

  ul {
    list-style: none;
  }

  .copyright,
  .termsofuse-privacy {
    color: rgba(255, 255, 255, 0.8);
    font-size: 0.8rem;
  }
}
</style>
