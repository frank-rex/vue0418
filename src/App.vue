<script setup>
import counterbutton from '@/components/counterbutton.vue'
let isDrawing = false;
let canvas;
let ctx;

function init() {
  canvas = document.createElement('canvas');
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;
  canvas.style.position = 'absolute';
  canvas.style.top = '0';
  canvas.style.left = '0';
  canvas.style.pointerEvents = 'none';
  document.body.appendChild(canvas);

  ctx = canvas.getContext('2d');
  ctx.strokeStyle = 'white';
  ctx.lineWidth = 2;
}

function startDrawing(event) {
  isDrawing = true;
  ctx.beginPath();
  ctx.moveTo(event.clientX, event.clientY);
}

function draw(event) {
  if (!isDrawing) return;
  ctx.lineTo(event.clientX, event.clientY);
  ctx.stroke();
}

function endDrawing() {
  isDrawing = false;
}

window.addEventListener('mousedown', startDrawing);
window.addEventListener('mousemove', draw);
window.addEventListener('mouseup', endDrawing);

init();

</script>

<template>
  <h3></h3>
  <div class="my-class">
  <a href="SupermarketView">
    <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/335024369_507390248269651_481113079401748469_n.jpg?stp=cp6_dst-jpg&_nc_cat=106&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=Uq1NjdBPMQgAX94EXoA&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfCraz5WdJSHUfD1_MmX9L6vXXGcQdmTSG1AsRGLHPdwEg&oe=644E0120" class="logoup" alt="lll logo"/>
  </a>
  <a href="ClassroomView">
    <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/334979866_607669337885007_5314857770609897713_n.jpg?stp=cp6_dst-jpg&_nc_cat=106&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=HJAaIdMjXmIAX8_mX5H&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfADWCpluyhrfHTVF_C8aPYlGaWSBqCq_cdMuHK-6SQWOg&oe=644D5050" class="logoup" alt="lll logo"/>
  </a>
</div>
  <div>
   <p></p>
   <p></p>
    <a href="MRT" target="_blank">
      <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/334649468_911727253283009_2413288863173424525_n.jpg?stp=cp6_dst-jpg&_nc_cat=102&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=GYnCMs07P3wAX-9vODx&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfANYKpp-kNzPOtPVMS3w20cEQReOvA3EkahMtVgNqA2TQ&oe=644E72D2" class="logo" alt="lll logo" />
    </a>
    <a href="RestaurantView" target="_blank">
      <img src="https://scontent.ftpe2-2.fna.fbcdn.net/v/t39.30808-6/334951579_1811685042565215_3884086571783012910_n.jpg?stp=cp6_dst-jpg&_nc_cat=102&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=xkWa8O6ptHoAX_OYnOJ&_nc_ht=scontent.ftpe2-2.fna&oh=00_AfCULeteAiDfnAhxra6NTrOMvqjZHVnxMRI2Nw1XyJrfnw&oe=644DAB1C" class="logo" alt="lll logo" />
    </a>
  </div>
  <HelloWorld msg="選擇想要練習的情境" />
  <h1>選擇想要練習的情境</h1>
  
</template>


<style scoped>
h1 {
    color: white;
  }
.logoup {
  height: 10em;
  padding: 3em;
  will-change: filter;
  transition: filter 300ms;
  transform: translateY(45px);
}
.logo {
  height: 10em;
  padding: 3em;
  will-change: filter;
  transition: filter 300ms;
  transform: translateY(40px);
}
.logo:hover {
  filter: drop-shadow(0 0 2em #BE9164);
}
.logoup:hover {
  filter: drop-shadow(0 0 2em #BE9164);
}
body {
  background-color: black;
}

</style>
