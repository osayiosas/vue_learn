<!-- Js -->

<script setup>
//  const myMessage = 'hello world'
//  const myNum = 100

//  function add (x, y) {
//         return x + y
//  }

// const myX = 'https://twitter.com/e_idiaghe'


//---------
// -dynmic binding 


const imageInfo = {
    src: 'https://collection.cloudinary.com/osaigbovo/e2b7599f564dcb0a0d8ec7662386b1d3?',
    alt: 'A generic square placeholder image with a white border around it, making it resemble a photograph.',
    width: 400,
    height: 400,
}


</script>

<!-- css -->

<style scoped>
   
</style>




<!-- Html -->

<template>

    <!-- <h1> {{ myMessage }} </h1>
    <h2>{{ myNum }}</h2>
    <h3> 2 + 2 = {{ 2 + 2 }}</h3>
    <h4>add two number:{{ add(2,10) }}</h4> -->

    <!-- <p> not allowed{{ const myName = 'osayi' }}</p> -->

    <!-- <a :href=" myX ">Twitter</a> -->

    <img :="imageInfo" />

</template>

