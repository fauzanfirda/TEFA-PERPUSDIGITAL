<template>
    <div class="container-fluid">
        <div class="row my-5">
            <div class="col-lg-6 mb-3">
                <nuxt-link to="/pengunjung/tambah">
                <div class="card bg-pengunjung rounded-5">
                        <div class="card-body">
                            <h2>pengunjung</h2>
                        </div>
                </div>
                </nuxt-link>
            </div>

            <div class="col-lg-6">
                <nuxt-link to="/buku">
                    <div class="card bg-buku rounded-5">
                        <div class="card-body">
                            <h2>cari buku</h2>
                        </div>
                    </div>
                </nuxt-link> 
          </div>
      </div>
    </div>

    <h2 class="mt-5" style="font-family: inter; margin-left: 20px;">STATISIK</h2>


    <div class="container-fluid">
        <div class="row my-5">
            <div class="col-lg-6 mb-3">
                <nuxt-link to="/pengunjung/tambah">
                <div class="card bg-warning rounded-5">
                        <div class="card-body">
                            <h2 class="pt-5">1000      pengunjung</h2>
                        </div>
                </div>
                </nuxt-link>
            </div>

            <div class="col-lg-6">
                <nuxt-link to="/buku">
                    <div class="card bg-primary rounded-5">
                        <div class="card-body">
                            <h2 class="pt-5">2000       buku</h2>
                        </div>
                    </div>
                </nuxt-link> 
          </div>
      </div>
    </div>
    <div>
        <Chart />
      </div>


      
      
</template>

<style scoped>
.card {
    height: 250px;
    box-shadow: 1px 1px 10px #424242
}
.card.bg-pengunjung {
    background-image:url(../assets/img/bg-home-kunjungan.jpeg);
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
    opacity: 50%;
} 
.card.bg-buku {  
    background:url(../assets/img/bg-home-cari-buku.jpg) no-repeat center center;
    background-size: cover;
    opacity: 50%;

}

</style>