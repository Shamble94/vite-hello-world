<script>
export default {
  data(){
    return{
      img: `vue.svg`
    }
  },
  methods:{
    getImage(path){
        return new URL(path, import.meta.url).href
    }
  }
}

</script>
<template>
  <div>
  </div>
    <img :src="getImage(`../assets/${img}`)" width="300px">
</template>