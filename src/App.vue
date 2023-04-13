<script>
import AppHeader from './components/AppHeader.vue';
import AppMainTop from './components/AppMainTop.vue';
import AppMainBottom from './components/AppMainBottom.vue';

export default {
  components: {
    AppHeader,
    AppMainTop,
    AppMainBottom
  }
}
</script>

<template>
<AppHeader />
<AppMainTop />
<AppMainBottom />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
</style>
