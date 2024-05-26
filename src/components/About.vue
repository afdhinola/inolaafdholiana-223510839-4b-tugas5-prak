<template>
    <div class="about">
        <History />
        <Project />
        <Footer />
    </div>
</template>

<script>
    import History from '../components/History.vue';
    import Project from '../components/Project.vue';
    import Footer from '../components/Footer.vue';

    export default {
        name : 'About',
        components: {
            History,
            Project,
            Footer,
        }
    }

</script>