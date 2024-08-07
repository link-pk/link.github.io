<script setup lang="ts">
// import HelloWorld from './components/HelloWorld.vue'
import { ref } from 'vue'
const list = ref(['2.png', '3.png', '4.png','2.png','vite.svg','4.png' ,'2.png','3.png','4.png'])
const odx = ref(0)
const listRunIndex = [0,1,2,5,8,7,6,3]
const run = (item: any) => {
  if(item !== 'vite.svg') return;
  console.log('run')
  setInterval(() => {
    odx.value++
    if (odx.value >= listRunIndex.length ) {
      odx.value = 0
    }
  }, 1000)

}

</script>

<template>
  <div class="content">
    <div class="box">
      <div class="box-item"  v-for="(item, index) in list" :key="index" :class="{'border-box': listRunIndex[odx] === index}">
        <img :src="`./../public/${item}`" alt="" @click="run(item)"/>
       </div>
      <!--  <img src="./../public/2.png" alt="" />
      </div>
      <div class="box-item">
        <img src="./../public/3.png" alt="" />
      </div>
      <div class="box-item">
        <img src="./../public/4.png" alt="" />
      </div>
      <div class="box-item">
        <img src="./../public/2.png" alt="" />
      </div>
      <div class="box-item">
        <img src="./../public/vite.svg" alt="" @click="run"/>
      </div>
      <div class="box-item">
        <img src="./../public/4.png" alt="" />
      </div>
      <div class="box-item">
        <img src="./../public/2.png" alt="" />
      </div>
      <div class="box-item">
        <img src="./../public/3.png" alt="" />

      </div>
      <div class="box-item">
        <img src="./../public/4.png" alt="" />
      </div> -->


    </div>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.content {
  height: 100vh;
  width: 100vw;
  background-color: #f5f5f5;
  display: flex;
  justify-content: center;
  align-items: center;
  background: url(1.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  background-attachment: fixed;

  .box {
    position: absolute;
    width: 100%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    margin-top: -26px;

    .box-item {
      width: calc(calc(100% - 50px) / 3);
      /* height: 300px; */
      /* padding-top: 100%; */
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
      border-radius: 10px;
      border: 1px solid transparent;
    
    


      img {
        width: 100%;
        height: 100%;
      }
    }

    .border-box {
      border: 1px solid transparent;
      background: linear-gradient(white, white) padding-box, repeating-linear-gradient(45deg, #FFDE00 0%, #FFDE00 4.6%, #3EAAFF 0, #3EAAFF 10%) 0rem 6.9rem
;
    }

    .box-item::before {
      content: '';
      display: block;
      padding-top: 100%;
    
    }
  }

}
</style>
