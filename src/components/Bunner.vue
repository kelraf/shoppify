<template>
    <div class="container-fluid m-0 p-0">
        <div class="row m-0">
            <div class="col-md-12 bunner p-0 pt-5 pb-5">
                <h1 class="bunner-header text-center pt-4">Shopify Help Center</h1>
                <h4 class="text-center pt-2">What are you looking for?</h4>

                <Form />
            </div>
        </div>
    </div>
</template>

<script>
import Form from '@/components/Form'
export default {
    components: {
        Form
    }
}
</script>

<style scoped>
    .bunner {
        background: whitesmoke;
        /* height: 40px; */
    }
    /* .bunner-header {

    } */
</style>