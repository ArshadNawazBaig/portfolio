<template>
  <div class="portfolio bg-gray-900 min-h-screen py-16">
        <div class="container mx-auto">
            <heading description="A FEW RECENT DESIGN AND CODING PROJECTS. WANT TO SEE MORE? EMAIL ME." span="My">Portfolio</heading>
            <div class="w-full md:w-5/6 mx-auto">
                <div class="mt-14 grid grid-flow-col grid-cols-1 grid-rows-9 md:grid-cols-3 md:grid-rows-3 gap-7 text-white">
                    <a href="#" class="bg-white text-white rounded h-48 bg-white relative group transition delay-1000 duration-300 ease-in-out" style="`background-image: url(${project.image})`" v-for="(project, index) in projects" :key="index">
                        <div class="invisible absolute bg-primary-100 w-full h-full rounded text-white flex justify-center items-center group-hover:visible">{{project.name}}</div>
                    </a>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
import Heading from './../../components/Heading/index.vue'
import Image from './../../assets/hero-image.jpg'
export default {
    data() {
        return {
            projects: [
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
                {name: 'project 1', image: Image},
            ]
        }
    },
    components: {
        Heading
    }
}
</script>

<style>

</style>