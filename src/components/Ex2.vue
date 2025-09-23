<script>
    export default { 
        data() {
            return {
                width: '200',
                height: '200',
                myImg: '/assets/me.png'
            }
        },
    }
</script>

<template>

    <!-- add code here -->
   <div id="img">
    <img v-bind:src="myImg" :width="width" :height="height"></img>
   </div>
</template>
