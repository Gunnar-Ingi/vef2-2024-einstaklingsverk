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
    margin: 5px;

    display: flex;
    justify-content: center;
    align-items: center;
    
    width: 25vw;
    height: 10vh;
    border-radius: 24px;
  }
  
</style>