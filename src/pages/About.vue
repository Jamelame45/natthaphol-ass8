<template>
    <div>
        <Navbar />

        <section class="about">

            <h1 class="heading"> about <span>me</span> </h1>

            <div class="row">

                <div class="info-container">

                    <h1>Manga Go</h1>

                    <div class="box-container">

                        <div class="box">
                            <h3> <span>name : </span>{{name}}</h3>
                            <h3> <span>founded : </span>{{age}}</h3>
                            <h3> <span>email : </span>{{email}}</h3>
                        </div>

                   

                    </div>

                    <a href="/profilewithcss/files/resume.pdf" class="btn"> download CV <i class="fas fa-download"></i>
                    </a>

                </div>

                <div class="count-container">

                   

                </div>

            </div>

        </section>

        <!-- about section ends -->

        <!-- skills section starts  -->

        <section class="skills">

            <h1 class="heading"> <span>my</span> Manga and Anime </h1>

            <div class="box-container">
                <div class="box">
                    <img src="images/action.jpg">
                    <h3>Action</h3>
                </div>
                <div class="box">
                    <img src="images/adventure.jpg">
                    <h3>adventure</h3>
                </div>
                <div class="box">
                    <img src="images/drama.webp">
                    <h3>drama</h3>
                </div>
                <div class="box">
                    <img src="images/romance.webp">
                    <h3>romance</h3>
                </div>
                <div class="box">
                    <img src="images/horror.jpg">
                    <h3>horror</h3>
                </div>
                <div class="box">
                    <img src="images/other.jpg">
                    <h3>other</h3>
                </div>
            </div>

        </section>

        <!-- skills section ends -->

        <!-- education section starts  -->

        <section class="education">


            <div class="box-container">

                <div class="box" v-for="e in study" :key="e.years">
                    <i class="fas fa-briefcase"></i>
                    <span>{{e.years}}</span>
                    <h3>{{e.school}}</h3>
                    <p>{{e.jobs}}</p>
                </div>

            </div>

        </section>
    </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
export default {
    components: { Navbar },
    data() {
        return {
            name: 'Manga Go',
            age: '15/10/2023',
            email: 'Natthaphol.lapc@bu.ac.th',

        }
    }
}
</script>

<style>

</style>