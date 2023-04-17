<script>
export default {
    name: "AppStyleCard",
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <img :src="image" alt="">
        <h4>{{ title }}</h4>        
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.card {
    width: calc(100% / 6 - 20px);
    object-fit: contain;
    margin: 10px;
}

h4 {
    color: white;
    max-width: 100px;
}

img {
    max-width: 100%;
    height: 100px;
    width: 100px;
}
</style>