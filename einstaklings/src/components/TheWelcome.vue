<script setup>
import WelcomeItem from './WelcomeItem.vue'
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
  <WelcomeItem>
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

<InfoCards>
      <p>
        MORE INFO ABOUT WHATEVER
    </p>
</InfoCards>
    
    <SectionItem v-if="blender">
      <p>
        Here are some 3d models, made in Blender.
      </p>
    </SectionItem>
    <div v-else></div>

    
<SectionItem v-if="mods">
      <p>
        Here are some game mods.
      </p>
    </SectionItem>
  <div v-else></div>

    <SectionItem v-if="art">
      <p>
        Here is some artwork.
      </p>
    </SectionItem>
    <div v-else></div>

  </WelcomeItem>

</template>
