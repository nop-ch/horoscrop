<template>
<div>
   <div class="h-full w-full d-flex justify-content-center align-items-center text-center text-light">
         <div style="display:flex ">
            <div class="col ">
               <div class="card" >
                  <img src="../../assets/images/card-1.jpg" class="card-img-top" alt="...">
                  <div class="card-body">
                     <h5 class="card-title">Card title</h5>
                     <p class="card-text">1111111111111111111111111111111111111111111111111111111111Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                     <a href="#" class="btn btn-primary">Go somewhere</a>
                  </div>
               </div>
            </div>
            <div class="col">
               <div class="card" >
                  <img src="../../assets/images/card-2.jpg" class="card-img-top" alt="...">
                  <div class="card-body">
                     <h5 class="card-title">Card title</h5>
                     <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                     <a href="#" class="btn btn-primary  mt-auto">Go somewhere</a>
                  </div>
               </div>
            </div>
            <div class="col">
               <div class="card" >
                  <img src="../../assets/images/card-3.jpg" class="card-img-top" alt="...">
                  <div class="card-body">
                     <h5 class="card-title">Card title</h5>
                     <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                     <a href="#" class="btn btn-primary  mt-auto">Go somewhere</a>
                  </div>
               </div>
            </div>

         </div>
     
   </div>
</div>
</template>

<script>
export default {
   getImgUrl(image) {
    return `../../assets/images/${image}.png`
   }   
}
</script>

<style scoped>
   .card{
      width: 320px;    
      height: 100%;
      margin: 0 auto;
      /* background-color: rgba(132, 101, 255, 0.428); */
      background-color: rgba(132, 101, 255, 0.7);
   }
   .btn-purple{
      background-color: rgb(175, 21, 230);
   }
   .card-body{
      display: flex;
      flex-direction: column;
   }

</style>