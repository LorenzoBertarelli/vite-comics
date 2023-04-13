<script>
export default {
    name: "AppMainTop"
}
</script>

<template>
    <main class="jumbo-top">
        <h1> --> Content goes here &lt-- </h1>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
    .jumbo-top {
        padding: 4rem;
        max-width: 100%;
        background-color: rgb(31, 31, 31);

        h1 {
            width: 1200px;
            margin: 0 auto;
            color: white;
            display: flex;
            align-items: center;
        }
    }
</style>