<template>
   <h1 :class="$style['m-class']" >
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vero, beatae? css module with $ sign (kabak-case)
   </h1> 

   <h1 :class="$style.anotherClass" >
    Lorem ipsum dolor sit. css module with $ sign (camelCase)
   </h1>
</template>

<style module> 
/* kabab-case */

.m-class {
    background: rgb(222, 120, 11);
    color: rgb(15, 16, 16);
}

.anotherClass {
    background: seagreen;
    color: rgb(15, 16, 16);
}
</style>