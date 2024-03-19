<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12">
                <h2 class="text-center my-4">RIWAYAT KUNJUNGAN</h2>
                <div class="my -3">
                    <input type="search" class="form-control form-control-lg rounded-5" planceholder="filter...">
                </div>
                <div class="my-3 text-muted">menampilkan 1 dari 1</div>
                <table class="table">
                    <thead>
                        <tr>
                            <td>#</td>
                            <td>NAMA</td>
                            <td>KEANGGOTAAN</td>
                            <td>WAKTU</td>
                            <td>KEPERlUAN</td>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>1.</td>
                            <td>Fauzan</td>
                            <td>Siswa</td>
                            <td>02 february 2007, 23.31.00</td>
                            <td>Baca</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>
    <nuxt-link to="../">
        <button type="submit" class="btn btn-dark btn-lg rounded-5 px-5">back</button>
    </nuxt-link> 
</template>

<style scoped>
.container-fluid {
    background-color: #DCB013;
    padding: 0 !important;
    margin: 0 !important;
}
.row, .col-lg-12 {
    margin: 0 !important;
    padding: 0 !important;
}
</style>