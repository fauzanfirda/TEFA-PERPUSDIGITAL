<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12">
                <h2 class="text-center my-4">BUKU</h2>
                <div class="my-3">
                    <form @submit.prevent="getBooks">
                        <input v-model="keyword" type="search" class="form-control rounded-5" placeholder="Mau baca apa hari ini">
                    </form>
                    
                </div>
                <div class="my-3 text-muted">menampilkan 2 dari 2</div>
                <div class="row">
                    <div v-for="(book, i) in books" :key="i" class="col-lg-2">
                        <div class="card-mb-4">
                            <div class="card-body">
                                <NuxtLink :to="`/buku/${book.id}`">
                                <img :src="book.cover" class="cover" alt="cover">
                                </NuxtLink>
                            </div>
                        </div>
                    </div>
                <nuxt-link to="../">
                    <button type="submit" class="btn btn-dark btn-lg mt-5 rounded-5 px-5">back</button>
                </nuxt-link>
            </div>
        </div>
        </div>
    </div>
</template>


<script setup>

const supabase = useSupabaseClient()
const books = ref([])

const keyword = ref('')

const getBooks = async () => {
    const { data, error } = await supabase.from('buku').select(`*, kategori(*)`)
    . ilike('judul', `%${keyword.value}`)
    if(data) books.value = data
}


onMounted(() => {
    getBooks()
})

</script>


<style scoped>
/* .card-body {
    width: 100%;
    height: 20em;
    padding: 0;
} */
.cover {
    width: 70%;
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

