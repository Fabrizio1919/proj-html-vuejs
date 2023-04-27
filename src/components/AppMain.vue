<script>
import Jumbotron from '../components/Jumbotron.vue';
import WorkColture from '../components/WorkColture.vue';
import UpgradeSkills from '../components/UpgradeSkills.vue';
import OnlineCourses from '../components/OnlineCourses.vue'
import PeopleHearts from './PeopleHearts.vue';
import GuideFree from '../components/GuideFree.vue';
import OurBlogs from '../components/OurBlogs.vue';
import EnterEmail from '../components/EnterEmail.vue'


export default {
    components: {
        Jumbotron,
        WorkColture,
        UpgradeSkills,
        OnlineCourses,
        PeopleHearts,
        GuideFree,
        OurBlogs,
        EnterEmail
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
    <EnterEmail></EnterEmail>
    
    
</template>


<style></style>