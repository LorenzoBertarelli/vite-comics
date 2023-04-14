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
}
</style>