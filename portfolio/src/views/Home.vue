<template>
        <v-container grid-list-sm class="heh">
            <!-- <div class="phrase"><span>Freelance designer and Illustrator</span></div> -->
            <v-layout row wrap>
                <v-flex xs12 sm6 md4 lg2 v-for="(project, index) in projects" :key="index">
                    <router-link v-bind:to="{ name: 'project', params: { 
                        title: project.title,
                        imgLink: project.imgLink,
                        client: project.client,
                        description: project.description
                        }}">
                        <v-flex>
                        <v-card>
                            <v-img class="img" v-bind:src="project.imgLink" height="300px" alt="Project image"></v-img>
                        </v-card>
                        </v-flex>        
                    </router-link>         
                </v-flex>
            </v-layout>
        </v-container>
</template>

<script>
import projects from '../components/projects.vue'

    export default {
        components: {
            'projects': projects
        },
        data() {
            return {
                projects: [
                    {title: 'INFOMERCIAL',client: 'Kaffesmeden', imgLink:'https://i.ibb.co/H4xnvZq/Screenshot-7.png',
                    description: 'Video infomercial project for a local cafe', alink: 'https://youtu.be/t35LsZ-bON0'},
                    {title: 'ADVENTURE',client: 'Self', imgLink:'https://i.ibb.co/n7gFzXq/bj.png',
                    description: 'Spare-time Illustration'},
                    {title: 'MINI ME',client: 'Academy project', imgLink:'https://i.ibb.co/tLVdXvP/Screenshot-1.png',
                    description: 'Vectorizing myself using Adobe Illustrator'},
                    {title: 'TOMBOY',client: 'Self', imgLink:'https://i.ibb.co/c6L3b9J/Screenshot-3.png',
                    description: 'Spare-time Illustration'},
                    {title: 'B-ROLL',client: 'Academy project', imgLink:'https://i.ibb.co/hWv4Jnt/Screenshot-5.png',
                    description: 'B-Roll footage excercise'},
                    {title: 'WARRIOR WITHIN',client: 'Self', imgLink:'https://i.ibb.co/t89xBHN/Screenshot-32.png',
                    description: 'Spare-time Illustration'},
                    
                    {title: 'DREAMY THOUGHTS',client: 'Self', imgLink:'https://i.ibb.co/GHpdTz3/v2.jpg',
                    description: 'Spare-time Illustration'},
                    {title: 'SOLAR WEB',client: 'Academy project', imgLink:'https://i.ibb.co/cccrfjN/Screenshot-4.png',
                    description: 'Educational web-application about our Solar system'},
                    {title: 'JOBLESS',client: 'Academy project', imgLink:'https://i.ibb.co/9N98gZL/Screenshot-2.png',
                    description: 'Job portal for students in and around Esbjerg'},
                    {title: 'STUDENT FOR A DAY',client: 'Academy project', imgLink:'https://i.ibb.co/M8VFr2x/Screenshot-8.png',
                    description: 'More like "Movie nights"'},
                    {title: 'EXHALE',client: 'Self', imgLink:'https://i.ibb.co/6bkMryw/dud.jpg',
                    description: 'Spare-time Illustration'},
                    {title: 'WEB-AD',client: 'Academy project', imgLink:'https://i.ibb.co/JmT6GKL/1.png',
                    description: 'Website serving as an advertisement for a line of products (phones in this case)'},
                    
                ]
            }
        },
    }
</script>

<style scoped>
.heh{
    margin: 0 auto;
    padding: 0 5px 30px 5px;
}
.phrase{
    text-align: center;
    font-family: 'din';
    padding-bottom: 10px;
}
.img {
    filter: grayscale(100%);;
    transition: all 200ms ease;
}
.img:hover {
    filter: grayscale(0%);;
}
</style>