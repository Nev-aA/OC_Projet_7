<template>
    <div class="create-post">
        <div class="header">
            <Navbar />
        </div>
        <div class="contentBar">
            <CreatePostMenu />
        </div>
    </div>
</template>

<script>
import Navbar from "../components/Navbar";
import CreatePostMenu from "../components/CreatePostMenu";

export default {
    name: "CreatePost",
    components: {
        Navbar,
        CreatePostMenu,
    },
};
</script>

<style lang="scss">
</style>