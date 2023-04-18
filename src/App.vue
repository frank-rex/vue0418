<script setup>
import counterbutton from '@/components/counterbutton.vue'

</script>


<template>
  <h3>     學習情境      </h3>
  
  
  <div>
    
    <a href="SupermarketView">
      <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/335024369_507390248269651_481113079401748469_n.jpg?stp=cp6_dst-jpg&_nc_cat=106&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=tDDGgl4nIT0AX8JVicy&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfCM_SotS9WjmDi99uTpF6xLlWWfjvhOIKJTesCSeExnyA&oe=643C34E0" class="logo" alt="rrr logo" />
    </a>
   
    <a href="ClassroomView">
      <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/334979866_607669337885007_5314857770609897713_n.jpg?stp=cp6_dst-jpg&_nc_cat=106&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=A1LwnUWZlvsAX_NKDyb&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfDE-dWU7Bw_NWQZjn2SLRaTlu1WXfpTuIaWNeBFwfQgBQ&oe=643B8410" class="logo" alt="lll logo" />
    </a>
   <p>
    SupermarketView | ClassroomView 
   </p>
   <p>
     .
   </p>
   <p>
     MRT | RestaurantView 
   </p>

    <a href="MRT" target="_blank">
      <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/334649468_911727253283009_2413288863173424525_n.jpg?stp=cp6_dst-jpg&_nc_cat=102&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=FcTDdZ8FEO0AX9yrobP&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfBV1yRJeBQmXY0UgbwMS1Q-bgMQZMnf8AAsXaR6ITk1IA&oe=643AAC52" class="logo" alt="lll logo" />
    </a>
    
    <a href="RestaurantView" target="_blank">
      <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/334951579_1811685042565215_3884086571783012910_n.jpg?stp=cp6_dst-jpg&_nc_cat=102&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=dZBlEvNlRFIAX_FLyPU&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfDF5RiTQdE3fMWwmxn0I_MU9Q5sEXMXASUpU4ynRApwfQ&oe=643BDEDC" class="logo" alt="lll logo" />
    </a>
    
  
   
    
  </div>
  <HelloWorld msg="選擇想要練習的情境" />
  <h1>選擇想要練習的情境</h1>
</template>


<style scoped>

.logo {
  height: 10em;
  padding: 3em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #da0000dd);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}

</style>
