<script>
import Jumbotron from '../components/Jumbotron.vue';
import WorkColture from '../components/WorkColture.vue';
import UpgradeSkills from '../components/UpgradeSkills.vue';
import OnlineCourses from '../components/OnlineCourses.vue'
import PeopleHearts from './PeopleHearts.vue';
import GuideFree from '../components/GuideFree.vue'
import OurBlogs from '../components/OurBlogs.vue'

export default {
    components: {
        Jumbotron,
        WorkColture,
        UpgradeSkills,
        OnlineCourses,
        PeopleHearts,
        GuideFree,
        OurBlogs
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
    <GuideFree></GuideFree>
    <OurBlogs></OurBlogs>
    
    
</template>


<style></style>