<script>
import Jumbotron from '../components/Jumbotron.vue';
import WorkColture from '../components/WorkColture.vue';
import UpgradeSkills from '../components/UpgradeSkills.vue';
import OnlineCourses from '../components/OnlineCourses.vue'
import PeopleHearts from './PeopleHearts.vue';

export default {
    components: {
        Jumbotron,
        WorkColture,
        UpgradeSkills,
        OnlineCourses,
        PeopleHearts
    },
    name: "AppMain"
}

</script>

<template>
    <Jumbotron></Jumbotron>
    <WorkColture></WorkColture>
    <UpgradeSkills></UpgradeSkills>
    <OnlineCourses></OnlineCourses>
    <PeopleHearts></PeopleHearts>
    
    
</template>


<style></style>