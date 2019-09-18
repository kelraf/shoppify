<template>
    <div class="form-cont pt-3 pb-3">
        <form>
            <input type="text" placeholder="Search The Document">
            <input type="button" value="Search" >
        </form>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>

    .form-cont {
        /* background: blue; */
    }
    form {
        /* background: red; */
        width: 40%;
        margin: auto;
        display: flex;
        flex-direction: row;
    }

    form input[type=text] {
        flex: 3;
        border-radius: 20px;
        margin: 0.5px;
        outline: none;
        border: .5 solid gray;
    }

    form input[type=button] {
        flex: 1;
        height: 50px;
        border-radius: 20px;
        outline: none;
        border: none;
    }
</style>