<template>

</template>

<script>
import getPlace from '../composables/getPlace.js'
import classroom from '../assets/place/classroom.glb?raw'
export default {
    setup(){
        const {init,loadmodles, animate} = getPlace(classroom)
        init()
        loadmodles()
        animate()
    }
}
</script>