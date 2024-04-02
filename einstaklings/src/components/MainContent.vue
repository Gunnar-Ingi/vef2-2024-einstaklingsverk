<script setup>
import GeneralItem from './GeneralItem.vue'
import SectionItem from './SectionItem.vue'
import InfoCards from './InfoCards.vue'
import BoxSmall from './BoxSmall.vue'
</script>

<script>
export default {
  data() {
  return {
    art: true,
    blender: true,
    mods: true
  }
}
}
</script>


<template>
  <GeneralItem>
    <h1>
        Gunj
    </h1>
    
  <div class="line-up">
    <button @click="blender = !blender">
      <BoxSmall>
        <p>
          3D ART
        </p>
      </BoxSmall>
    </button>

    <button @click="art = !art">
      <BoxSmall>
        <p>
          2D ART
        </p>
      </BoxSmall>
    </button>

    
  <button @click="mods = !mods">
   <BoxSmall>
        <p>
          GAME MODS
       </p>
    </BoxSmall>
  </button>

  </div>
    
    <SectionItem v-if="blender">
      
      <img src="/test.png"/>
          
    <InfoCards>
          <p>
            Made in Blender
          </p>
          <ul> 
            <li>143 verts</li>
            <li>279 edges</li>
            <li>279 faces</li>
          </ul>
    </InfoCards>
    </SectionItem>
    <div v-else></div>

    
<SectionItem v-if="mods">
      <p>
        Here are some game mods.
      </p>
    </SectionItem>
  <div v-else></div>

    <SectionItem v-if="art">
      <img src="/test2.png"/>
      
    <InfoCards>
          <p>
            Made in Procreate
          </p>
    </InfoCards>
    </SectionItem>
    <div v-else></div>

  </GeneralItem>

</template>


<style scoped>
button {
  background-color: transparent;
  border: 1px;

  max-width: 256px;
  
  display: flex;
  }

  img {
    display: block;
    max-width: 400px;
    max-height: 400px;
    height: auto;
    width: auto;
  }
  
</style>
