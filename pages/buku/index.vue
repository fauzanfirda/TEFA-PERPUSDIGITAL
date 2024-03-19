<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12">
                <h2 class="text-center my-4">BUKU</h2>
                <div class="my-3">
                    <input type="search" class="form-control rounded-5" placeholder="Mau baca apa hari ini">
                </div>
                <div class="my-3 text-muted">menampilkan 3 dari 3</div>
                <div class="row">
                    <div class="col-lg-2">
                        <div class="card mb-3">
                                <div class="card-body">
                                    <img src="~/assets/img/Teluk-Alaska.jpg" class="cover1">
                                </div>
                        </div>
                    </div>
                    <div class="col-lg-2">
                        <div class="card mb-3">
                            <nuxt-link to = "/buku/des">
                            <div class="card-body">
                                <img src="~/assets/img/Teluk-Alaska.jpg" class="cover1" alt="cover 1">
                            </div>
                            </nuxt-link>
                        </div>
                    </div>
                    <div class="col-lg-2">
                        <div class="card mb-3">
                            <div class="card-body">
                                <img src="~/assets/img/Teluk-Alaska.jpg" class="cover1" alt="cover 1">
                            </div>
                        </div>
                    </div>
                </div>
                <nuxt-link to="../">
                    <button type="submit" class="btn btn-dark btn-lg rounded-5 px-5">back</button>
                </nuxt-link>
            </div>
        </div>
    </div>
</template>

<style scoped>
/* .card-body {
    width: 100%;
    height: 20em;
    padding: 0;
} */
.cover1 {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 0 30;
}
.container-fluid {
    background-color:  #B9B8B8;
    padding: 0 !important;
    margin: 0 !important;
} 
.btn-dark{
    display: flex;
    justify-content:flex-end;
}
</style>

