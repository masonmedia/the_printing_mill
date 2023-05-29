<script setup>

</script>

<template>
    <nav class="navbar bg-light fixed-top p-3 border-bottom">
        <div class="container-fluid">
            <a class="navbar-brand fs-5 fw-900 pb-0 border-top-0 border-end-0 border-start-0" href="#"
            style="border: solid 5px #DC3545;">TPM</a>
            <!-- <a class="navbar-brand fs-5 fw-900 bg-dark text-light p-2 rounded-4" href="#">TPM</a> -->

            <ul class="nav justify-content-end align-items-center ms-auto d-none d-lg-flex">
  <li class="nav-item">
    <a class="nav-link" aria-current="page" href="#">Home</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">About</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Services</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Reviews</a>
  </li>
  <li class="nav-item">   
        <a class="nav-link" href="#">
            <button class="btn btn-dark rounded-5 px-3">
                Contact Us
            </button>
        </a>
  </li>
</ul>
<div class="d-lg-none">
            <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar"
                aria-controls="offcanvasNavbar">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
                <div class="offcanvas-header">
                    <h5 class="offcanvas-title" id="offcanvasNavbarLabel">The Printing Mill</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                </div>
                <div class="offcanvas-body d-flex flex-column justify-content-end align-items-start p-4">
                    <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">About</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Services</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Contact</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>


        </div>
    </nav>
</template>

<style lang="scss" scoped>
a, .nav-item {
    color: inherit;
    font-size: 17px;
}

.offcanvas-body .nav-item {
    font-size: 7vmin;
    line-height: 7vmin;
    font-weight: 900;
    letter-spacing: -2px;
}
</style>