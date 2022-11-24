<script setup>
  import { ref } from 'vue'
  import  CardHoroScrope  from './cards/CardHoroScrope.vue'
  defineProps({
    msg: String
  })
  const message = ref()

  console.log(message.value);
  function onInput(event){
    console.log(event.target.tagName)
  }
</script>

<template>
  <section>
    <div class="showcase" >
      <div class="absolute" style="z-index: 1;">
        <CardHoroScrope />
      </div>
        <video  autoplay muted loop id="myVideo">
          <source src="../assets/videos/nightsky.mp4" type="video/mp4">
          <source src="movie.ogg" type="video/ogg">
          Your browser does not support the video tag.
        </video>
    </div>

  </section>
</template>

<style scoped>
.video-container{
  position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;

}
#myVideo {
  min-width: 100%;
	min-height: 100%;

  width: 100vw;
  position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
	object-fit: cover;
}

.showcase {
	height: 100vh;
}
</style>
