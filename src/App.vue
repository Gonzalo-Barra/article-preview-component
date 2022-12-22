<template lang="">
  <main>
    <div class="card">
      <div >
        <img class="image" src="/images/drawers.jpg" alt="flowers" />
      </div>
      <div class="text">
        <h1>
          Shift the overall look and feel by adding these wonderful touches to
          furniture in your home
        </h1>
        <p>
          Ever been in a room and felt like something was missing? Perhaps it
          felt slightly bare and uninviting. I’ve got some simple tips to help
          you make any room feel complete.
        </p>
      </div>
      <buttonCard />
    </div>

  </main>
</template>
<script setup>

import buttonCard from './components/buttonCard.vue'


</script>
<style >
main{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #f0f0f0;
}
.card{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  border-radius: 15px;
  width: 325px;

}
.image{
  width: 100%;
  height: auto;
  border-radius: 15px 15px 0 0;
}
.text{
  padding:30px 37px 30px 37px;
  Font-size: 15px;
}

.text h1{
  color:  hsl(217, 19%, 35%);
  font-weight: 700;
  Font-size: 15px;
  font-family: 'Manrope', sans-serif;
  padding-bottom: 25px;
  
}

.text p{
  color: hsl(214, 17%, 51%);
  Font-size: 13px;
  font-weight: 500;
  font-family: 'Manrope', sans-serif;
  
}

</style>
