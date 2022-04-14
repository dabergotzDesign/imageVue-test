<template>
  <main>
    <h2>Image</h2>

    <Image 
    v-for="(img, index) in imgData.slice(0,3)"
    :imgData="imgData"
    :key="index"
    :index="index"
    :skillIcons="icon"
    />

  </main>
</template>
<script>
import Image from '@/components/Image.vue'

export default {
  name:'gallery',
  props: ['imgData','index'],
  components: {
    Image
    }
}
  
</script>

