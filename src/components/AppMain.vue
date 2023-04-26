<script>
import Jumbotron from '../components/Jumbotron.vue';
import WorkColture from '../components/WorkColture.vue';
import UpgradeSkills from '../components/UpgradeSkills.vue';
import OnlineCourses from '../components/OnlineCourses.vue'

export default {
    components: {
        Jumbotron,
        WorkColture,
        UpgradeSkills,
        OnlineCourses
    },
    name: "AppMain"
}

</script>

<template>
    <Jumbotron></Jumbotron>
    <WorkColture></WorkColture>
    <UpgradeSkills></UpgradeSkills>
    <OnlineCourses></OnlineCourses>
    
    
</template>


<style></style>