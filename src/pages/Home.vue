<template>
    <div>
        <Navbar />
        <section class="home">
            <div class="image">
                <img src="images/profile.webp" alt="">
            </div>
            <div class="content">
                <h3>Hi, Wellcome to {{name}}</h3>
                <span>{{motto}}</span>
                <p>{{content}}</p>
                <router-link to="/about" class="btn"> about me <i class="fas fa-user"></i> </router-link>
            </div>
        </section>
    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components: { Navbar },
    data() {
        return {
            name: 'Manga Go',
            motto: 'Manga is LIFE',
            content: ' We have many manga to choose from.',
        }
}
}
</script>

<style>

</style>