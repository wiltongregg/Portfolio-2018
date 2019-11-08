<template>
    <footer>
        <span> {{ footerText }} </span>
    </footer>
</template>

<script>
    export default {
        data() {
            return {
                footerText: 'Edvin Milos May 2019'
            }
        }
    }
</script>

<style lang="scss" scoped>
    footer {
        background: rgb(213, 249, 255);
        padding: 10px;
        text-align: center;
    }
</style>