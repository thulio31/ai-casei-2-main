<template>
  <div>
    <banner />
    <Catalogo />
    <Flag />

  </div>
</template>

<script>
import Flag from '../components/Flag.vue'
import Banner from '../components/Banner.vue'
import Catalogo from '@/components/Catalogo.vue'

export default{
  name: 'Home',
  components:{
    Flag,
    Banner,
    Catalogo,
  }  
}
</script>