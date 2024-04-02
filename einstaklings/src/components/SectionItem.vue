<template>
    <section>
        <slot></slot>
    </section>
</template>


<style scoped>
section {
    background-color: #7CE9F3;
    color: #000;
    transition: 0.4s;
    padding: 10px;
    margin: 10px;
    
    display: flex;
    width: 70vw;
    height: 50vh;
    flex-wrap: wrap;
    border-radius: 24px;
    max-width: 1024px;
  }
  
</style>