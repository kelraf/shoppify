<template>

    <div v-if="welcome_artical_one.length == 2" class="row">
        <div v-for="article in welcome_artical_one" :key="article.id" class="col-md-6">
            <div class="col-md-12 article-cont">
                <router-link to="/" class="article">
                    <div class="container-fluid">
                        <div class="row">
                            <div class="col-3">
                                <i class="fa fa-user fa-2x"></i>
                            </div>
                            <div class="col-9">
                                <div class="row">
                                    <h5> {{ article.title }} </h5>
                                </div>
                                <div class="row">{{ article.article }}</div>
                            </div>
                        </div>
                    </div>
                </router-link>
            </div>
        </div>
    </div>

    <div v-else-if="welcome_artical_one.length == 3" class="row">
        <router-link to="/tstu" v-for="article in welcome_artical_one" :key="article.id" class="col-md-4">{{ article.article }}</router-link>
    </div>

    <div v-else-if="welcome_artical_one.length == 6" class="row">
        <router-link to="/diqu9i" v-for="article in welcome_artical_one" :key="article.id" class="col-md-2">{{ article.article }}</router-link>
    </div>

    <div v-else class="row">
        <router-link to="/ndwuqh" v-for="article in welcome_artical_one" :key="article.id" class="col-md-12">{{ article.article }}</router-link>
    </div>

</template>

<script>
export default {
    data() {
        return {
            welcome_artical_one: [
                {
                    id : 1,
                    icon: "fa fa-user fa-2X",
                    title: "Your Title One",
                    article: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore ."
                },
                {
                    id : 2,
                    title: "Your Title Two",
                    article: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore."
                }
            ]
        }
    }
}
</script>

<style scoped>
    i {
        color: rgb(27, 27, 110);
    }
    h5 {
        color: rgb(27, 27, 110);
    }
    .article-cont {
        transition-duration: .5s;
        border-radius: 5px;
         position: relative;
    }

    .article-cont:hover {
        top: -3px;
        box-shadow: 5px 10px 20px rgba(0, 0, 0, 0.5);
        border: 2px solid rgb(27, 27, 110);

    }

    .article {
        display: inline-block;
        text-decoration: none;
        color: black;
        padding-top: 10px;
        padding-bottom: 10px;
    }
    
</style>