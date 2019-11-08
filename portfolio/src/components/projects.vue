<template>
    <div>
        <ul>
            <li v-for="(item, index) in projects" :key="index" v-on:click="item.show = !item.show">
                <p>{{item.name}}</p>
                <p v-show="item.show">{{item.client}}</p>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                projects: [
                    { name: 'mini me', client: 'client: self', show: false },
                    { name: 'video cv', client: 'client: self', show: false },
                    { name: 'infomercial', client: 'client: Kaffesmedden', show: false },
                    { name: 'web-shop', client: 'client: self', show: false }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
ul {
    display: flex;
    max-width: 1000px;
    margin: 20px auto;
    padding: 10px;
    box-sizing: border-box;
}
li {
    list-style: none;
    padding: 20px;
    margin: 10px;
    text-align: center;
    border: 1px solid rgb(197, 74, 125);
    flex-grow: 1;
    flex-basis: 200px;
}
</style>