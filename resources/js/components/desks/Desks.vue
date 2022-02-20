<template>
    <div>
        <h1>Доски</h1>
        <div class="row">
            <div class="col-lg-4">
                <div class="card mt-3">
                    <a href="#" class="card-body">
                        <h5 class="card-title">Заголовок карточки</h5>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Desks",
    data(){
        return {
            desks:[]
        }
    },
    mounted() {
        axios.get('/api/V1/desks')
        .then(res=>{
            console.log(res)
        })
    }
}
</script>

