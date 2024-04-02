<template>
    <div class="item">
    <section>
        <slot></slot>
    </section>
</div>
</template>


<style scoped>
.item {
    background-color: #ED345B;
    color: #000;
    transition: 0.4s;
    padding: 10px;
    margin: 10px;
    
    display: flex;
    width: 30vw;
    height: 10vh;
    flex-wrap: wrap;
    border-radius: 24px;
  }
  
</style>