<template>
    <div class="item">
    <section>
        <slot></slot>
    </section>
</div>
</template>


<style scoped>
.item {
    background-color: #8E0D7F;
    color: #000;
    transition: 0.4s;
    padding: 10px;
    
    display: flex;
    width: 25vw;
    height: 25vh;
    flex-wrap: wrap;
    border-radius: 24px;
  }
  
</style>