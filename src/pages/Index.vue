<template>
    <Layout>
        <Block />
    </Layout>
</template>

<script>
import Block from "../components/Block.vue";

export default {
    components: {
        Block,
    },
    metaInfo: {
        title: "Hello, world!",
    },
};
</script>

<style>
.home-links a {
    margin-right: 1rem;
}
</style>
