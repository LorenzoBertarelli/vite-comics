<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    text: "MOVIE",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    text: "CFANS",
                    url: "#",
                    current: false
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="title">
            <a href="">
                <img src="../assets/img/dc-logo.png" alt="">
            </a>
            <nav>
                <ul class="list-header">
                    <li v-for="(link,index) in links" :key="index" :class="link.current ? 'color-list' : ''">
                        <a href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
.title {
    max-width: 1200px;
    margin: 0 auto;
    height: 150px;
    list-style: none;
    @include flex(row, center, center);
    justify-content: space-between;
    
    ul {
        display: flex;
    }

    li {
        margin: 0.5rem;
        list-style: none;
        padding: 64px 0;

        a {
            color: $text-color;
            text-decoration: none;
        }

        &.color-list,
        &:hover {
          color:$primary;
          border-bottom: 3px solid currentColor;
          height: 100%;
          a {
            color: currentColor;
          }
        } 
    }
}
</style>
