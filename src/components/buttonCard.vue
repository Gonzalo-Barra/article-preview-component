<template lang="">
  <div class="button-class">
    <div class="button-class--passive" v-if="ocultartDiv">
    <div class="button-class--passive-info" >  <img class="button-class--passive-avatar" src="/images/avatar.jpg" alt="avatar" />
      <p class="button-class--passive-infotext"><strong>Michelle Appleton</strong> <br/>28 jun 2020</p></div>
      <img
        class="button-share"
        @click="cambiarMostrarDiv"
        src="/images/icon-share.svg"
        alt="button share"
      />
    </div>
    <div class="button-class--active" v-if="mostrarDiv">
      <p>share</p>
      <div><img  class="button-class--active-icons" src="/images/icon-facebook.svg" alt="icon facebook" />
      <img class="button-class--active-icons" src="/images/icon-twitter.svg" alt="icon twitter" />
      <img class="button-class--active-icons" src="/images/icon-pinterest.svg" alt="icon pinterest" /></div>
      <img
        class="button-share"
        @click="cambiarMostrarDiv"
        src="/images/icon-share.svg"
        alt="button share"
      />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      mostrarDiv: false,
      ocultartDiv: true,
    };
  },
  methods: {
    cambiarMostrarDiv() {
      this.mostrarDiv = !this.mostrarDiv;
      this.ocultartDiv = !this.ocultartDiv;
    },
  },
};
</script>

<style>
.button-class {

  width: 100%;
  display: flex;
  
}

.button-share{
  width:30px;
  height: 30px;
  margin-left: 40px ;
  padding: 9px;
  border-radius: 100%;
background-color: hsl(210, 46%, 95%);

}

.button-class--passive {
  border-radius: 100%;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  background-color: white;

}
.button-class--passive-info{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-around;
}

.button-class--passive-infotext{
  color: hsl(0, 0%, 59%);
  font-size: 12px;
  margin-left: 15px;
  font-family: 'Manrope', sans-serif;
  font-weight: 500;

}
.button-class--passive-infotext strong{
  color:  hsl(214, 17%, 51%);
  font-weight: 700;

}
.button-class--passive-avatar {
  width: 40px;
  height: 40px;

  border-radius: 100%;

}

.button-class--active {

  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  background-color: hsl(217, 19%, 35%);
}

.button-class--active img {
  width: 30px;
  height: 30px;
  margin: 10px;
  
}

.button-class--active p {
  color: hsl(212, 23%, 69%);
  font-size: 12px;
  font-family: 'Manrope', sans-serif;
  font-weight:5 00;
}	

.button-class--active .button-class--active-icons{
  width: 20px;
  height: 20px;



}	

</style>
