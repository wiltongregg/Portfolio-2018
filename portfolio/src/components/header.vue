<template>
    <header>
        <nav>
        <v-toolbar flat app class="toolbar" height="150px">
                <div class="links1">
                    <router-link class="nav" to="/"> work </router-link>
                    <router-link class="nav" to="/about"> about </router-link>
                </div>
                
                <v-spacer></v-spacer>
                <router-link class="nav" to="/"><img id="logo" src="../assets/logo5.png" width="100px" alt="Website logo"></router-link>
                <v-spacer></v-spacer>
                <div class="links2">
                    <a href="https://www.instagram.com/milos.edvin/" target="_blank"><div class="ig"></div></a>
                    <a href="https://www.linkedin.com/in/edvin-milos-07697111a/" target="_blank"><div class="in"></div></a>
                </div>
                
        </v-toolbar>
        </nav>
    </header>
</template>

<script>
    export default {
        data() {
            return {

            }
        }
    }
</script>

<style lang="scss" scoped>
.toolbar{
  background: rgb(255, 252, 252);
}
.nav{
    text-decoration: none;
    color: #282828;
    font-weight: 500;
    font-size: 1.2em;
    font-family: 'gothamB';
    margin-right: 10px;
    transition: 200ms;
}
.nav:hover{
    color: #e90000;
}
.ig, .in{
    transition: 200ms;
    margin-left: 10px;
}
.ig{
    background: url('../assets/instagram.png');
    width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}
.in{
    background: url('../assets/linkedin1.png');
    width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}
.ig:hover{
    background: url('../assets/instagramRed.png');
        width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}
.in:hover{
    background: url('../assets/linkedinRed.png');
        width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}
.links1{
    width: 200px;
    padding: 0;
    margin: 0;
}
.links2{
    width: 200px;
    padding: 0;
    margin: 0;
    text-align: right;
}
</style>