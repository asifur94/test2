<template>

    
    <courseAll v-for="course in courses" :key="course.id" :course="course">

                    

    </courseAll>


</template>


<script>
import axios from 'axios';
export default {
    data() {
        return {
            courses: [],
            names: [],

        }
    },
    mounted() {
        axios.get('http://test.test/api/course')
            .then(response => {
                console.log(response.data);
                this.courses = response.data

            })

    },
}
</script>