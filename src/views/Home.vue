<template>
  <div>
    <Flag />
    <introducao />
    <Catalogo />
    

  </div>
</template>

<script>
import Flag from '../components/Flag.vue'
import Banner from '../components/Banner.vue'
import Catalogo from '@/components/Catalogo.vue'
import introducao from '@/components/introducao.vue';

export default{
  name: 'Home',
  components:{
    Flag,
    introducao,
    Banner,
    Catalogo,
  }  
}
</script>