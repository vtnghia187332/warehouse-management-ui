<template>
    <div>
        <TheHeader class="main-header clearfix"></TheHeader>
        <div class="body-under-header">
            <TheNavBar class="main-navbar"></TheNavBar>
            <TheBody class="main-body"></TheBody>
        </div>
    </div>
</template>

<script>
import TheHeader from './TheHeader.vue';
import TheNavBar from './TheNavBar.vue';
import TheBody from './TheBody.vue';
export default {
    components: {
        TheBody, TheNavBar, TheHeader
    }
}
</script>
<style scoped>
/* header */
.main-header {
    top: 0;
    right: 0;
    left: 0;
    border-bottom: 2px solid #5abaad;
    background-color: #fff;
    height: 40px;
    z-index: 99;
    position: relative;
    max-height: 100px;
}

.clearfix {
    zoom: 1;
}

.body-under-header {
    position: relative;
    height: calc(100vh - 40px);
}

/* navbar */
.main-navbar {
    width: 256px;
    height: 100%;
    position: absolute;
    display: block;
}

/* body */
.main-body {
    word-break: break-word;
    background: #eff3f7;
    height: 100%;
    position: relative;
    min-height: 889px;
    margin-left: 256px;
}
</style>