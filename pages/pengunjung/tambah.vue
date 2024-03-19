<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12">
                <h2 class="text-center my-4">ISI BUKU KUNJUNGAN</h2>
                <from>
                    <div class="mb-3">
                        <input type="text" class="form-control form-control-lg rounded-5" placeholder="NAMA...">
                    </div>
                 <div class="mb-3">
                    <select class="form-control from-control-lg form-select rounded-5">
                        <option value="">KETERANGAN</option>
                        <option value="Siswa">Siswa</option>
                        <option value="Guru">Guru</option>
                        <option value="Staf">Staf</option>
                        <option value="Umum">Umum</option>
                    </select>
                 </div>
                 <div class="mb-3">
                
                        <div class="mb-4">
                            <select class="form-control form-control-lg form-select rounded-5 mb-2">
                                <option value="">TINGKAT</option>
                                <option value="X">X</option>
                                <option value="XI">XI</option>
                                <option value="XII">XII</option>
                                <option value="Umum">Umum</option>
                            </select>
                        </div>
                    
                 </div>
                 <div class="mb-3">

                        <div class="mb-4">
                            <select class="form-control form-control-lg form-select rounded-5 ,b-2">
                                <option value="">KELAS</option>
                                <option value="PPLG">PPLG</option>
                                <option value="TJKT">TJKT</option>
                                <option value="TSM">TSM</option>
                                <option value="DKV">DKV</option>
                                <option value="TOI">TOI</option>
                            </select>
                        </div>
                    
                </div>
                <div class="mb-3">
                    <select class="from-control form-control-lg form-select rounded-5">
                        <option value="">KEPERLUAN</option>
                        <option value="baca">BACABUKU</option>
                        <option value="pinjam">PINJAM BUKU</option>
                        <option value="kembalikan">KEMBALIKAN BUKU</option>
                    </select>
                </div>
                </from>
                <nuxt-link to="/pengunjung">
                    <button type="submit" class="btn btn-dark btn-lg rounded-5 px-5">KIRIM</button>
                </nuxt-link>   
                        <nuxt-link to="../">
                            <button type="submit" class="btn btn-dark btn-lg rounded-5 px-5" style="float: right;">back</button>
                        </nuxt-link> 
                 </div>
            </div>
        </div>
</template>


<style scoped>
.container-fluid {
    background-color: #F31ED1;
    padding: 0 !important;
    margin: 0 !important;
}
.row, .col-lg-12 {
    margin: 0 !important;
    padding: 0 !important;
}
</style>