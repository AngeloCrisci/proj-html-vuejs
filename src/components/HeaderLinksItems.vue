<script>

export default {
    data() {
        return {

        }
    },
    props: {
        linkLabel: {
            type: String,
            require: true
        },
        linkUrl: {
            type: String,
            required: true
        }
    }
}
</script>

<template>
    <li>
        <a href="linkUrl">{{ linkLabel }}</a>
    </li>
</template>

<style lang="scss" scoped>
    a {
        color: white;
        text-decoration: none;
        font-weight: bold;
        font-size: 1.1rem;
        padding-bottom: 10px;

        &:hover {
            border-bottom: 3px solid white;
        }
    }
</style>