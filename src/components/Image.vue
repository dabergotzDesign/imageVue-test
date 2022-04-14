<template>
  <main class="imageContainer">
    <ImageIcon />
    <div class="name">{{ imgData[index].name }}</div>
  </main>
</template>
<script>
import ImageIcon from '@/components/ImageIcon.vue'


export default {
  name: 'Image',
  props: ['imgData','index'],
   components:{
        ImageIcon
    }
}

</script>