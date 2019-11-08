<template>
    <div>
        <div class="text">
            <h1> {{project.title}} </h1>
            <h2> Client :: {{project.client}} </h2>
            <br><br>
            <p> {{project.description}} </p>
        </div>
        <v-img v-bind:src="project.imgLink" class="img" alt="Project image"></v-img>
        <div>
            <p> <a v-bind:href="project.alink">yo</a> HELLOOO </p>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            var project = this.$route.params
            return {
                show: false,
                project: {
                    title: project.title,
                    imgLink: project.imgLink,
                    client: project.client,
                    description: project.description,
                    alink: project.link
                }
            }
        },
    }
</script>

<style lang="scss" scoped>
.text{
    padding: 40px 50px;
}

</style>