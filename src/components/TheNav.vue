<script setup>
// image paths
function getImageUrl(name, ext) {
  return new URL(`../assets/img/${name}.${ext}`, import.meta.url).href
}
</script>

<template>
    <nav class="navbar bg-light fixed-top p-3 border-bottom">
        <div class="container-fluid">
            <!-- <a class="navbar-brand fs-5 fw-900 ls-base pb-0 border-top-0 border-end-0 border-start-0" href="#"
            style="border: solid 5px #DC3545;">TPM</a> -->
            <router-link to="/">
                <img class="navbar-brand" style="width: 200px" :src="getImageUrl('tpm_logo_h', 'png')" alt="">
            </router-link>
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
                    <a class="nav-link" href="mailto:info@theprintingmill.com" target="_blank">
                        <button class="btn btn-dark rounded-5 px-3">Contact Us</button>
                    </a>
                </li>
            </ul>
            <div class="d-lg-none">
                <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasRight"
                    aria-controls="offcanvasRight">
                    <span class="navbar-toggler-icon"></span>
                </button>

                <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasRight" aria-labelledby="offcanvasRightLabel">
                    <div class="offcanvas-header border-bottom">
                        <!-- <h5 class="offcanvas-title fw-bold ls-base text-secondary" id="offcanvasRightLabel">The Printing Mill</h5> -->
                        <img class="navbar-brand p-2" style="width: 200px" :src="getImageUrl('tpm_logo_h', 'png')" alt="">
                        <button type="button" class="btn-close border-0" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                    </div>
                    <div class="offcanvas-body">
                        <ul class="navbar-nav pe-3">
                            <li class="nav-item">
                                <a class="nav-link" data-bs-dismiss="offcanvas" aria-current="page" href="#">Home</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" data-bs-dismiss="offcanvas" href="#">About</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" data-bs-dismiss="offcanvas" href="#">Services</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" data-bs-dismiss="offcanvas" href="mailto:info@theprintingmill.com" target="_blank">Contact</a>
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

.offcanvas-body {
    padding: 50vh 30px 0;
}

.offcanvas-body .nav-item a {
    font-size: 50px;
    line-height: 45px;
    font-weight: 900;
    letter-spacing: -2px;
}
</style>