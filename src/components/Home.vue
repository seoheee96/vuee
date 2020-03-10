<template>
<div>
<center>
  <b-jumbotron header="Bespin 차량 예약 시스템" lead="원하는 시간대에 원하는 차량을 예약해보세요!" id="container">
    <p>Learn Do Share</p>
    <b-button variant="primary" to="register">회원가입하러가기</b-button>
  </b-jumbotron>
  </center>    
  <b-card-group id="card-g"> 

    <b-card
      title="현대 자동차 베뉴" 
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
      id="card1"
    >
    <hr>
    <img src="@/assets/car1.png" style="max-width: 15rem;">
      <b-card-text id="cardtxt">
      <p>
       가격 : <b>하루 73492원</b><br> 
       연비 : <b>11.3~16.1km</b><br> 
       도심주행에 적합한 안정적이고 편안한 주행성능<br> 
       진보된 첨단 지능형 주행 안전 기술 및 편의사양<br> 
      </p>
      </b-card-text>
      <b-button href="#" variant="primary">예약하러 가기</b-button>
    </b-card>
    <b-card
      title="람보르기니"
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
      id="card2"
    >
    <hr>
    <img src="@/assets/car2.png" style="max-width: 15rem;">
      <b-card-text id="cardtxt">
      <p>
       가격 : <b>하루 200만원</b><br> 
       연비 : <b>11.3~16.1km</b><br> 
       비싼 차이니까 조심히 탑시다.<br> 
       진보된 첨단 지능형 주행 안전 기술 및 편의사양<br> 
      </p>
      </b-card-text>

      <b-button href="#" variant="primary">예약하러 가기</b-button>
    </b-card>
    
    <b-card
      title="Card Title"
      img-src="https://picsum.photos/600/300/?image=25"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
      id="card2"
    >
      <b-card-text>
        Some quick example text to build on the card title and make up the bulk of the card's content.
      </b-card-text>

      <b-button href="#" variant="primary">예약하러 가기</b-button>
    </b-card>
    <b-card
      title="Card Title"
      img-src="https://picsum.photos/600/300/?image=25"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
      id="card2"
    >
      <b-card-text>
        Some quick example text to build on the card title and make up the bulk of the card's content.
      </b-card-text>

      <b-button href="#" variant="primary">예약하러 가기</b-button>
    </b-card>
    </b-card-group>

     <b-card-group id="card-g"> 
    <b-card
      title="현대 자동차 베뉴" 
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
      id="card1"
    >
    <hr>
    <img src="@/assets/car1.png" style="max-width: 15rem;">
      <b-card-text id="cardtxt">
      <p>
       가격 : <b>하루 73492원</b><br> 
       연비 : <b>11.3~16.1km</b><br> 
       도심주행에 적합한 안정적이고 편안한 주행성능<br> 
       진보된 첨단 지능형 주행 안전 기술 및 편의사양<br> 
      </p>
      </b-card-text>

      <b-button to="/reservation" variant="primary">예약하러 가기</b-button>
    </b-card>
    <b-card
      title="Card Title"
      img-src="https://picsum.photos/600/300/?image=25"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
      id="card2"
    >
      <b-card-text>
        Some quick example text to build on the card title and make up the bulk of the card's content.
      </b-card-text>

      <b-button href="#" variant="primary">예약하러 가기</b-button>
    </b-card>
    
    <b-card
      title="Card Title"
      img-src="https://picsum.photos/600/300/?image=25"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
      id="card2"
    >
      <b-card-text>
        Some quick example text to build on the card title and make up the bulk of the card's content.
      </b-card-text>

      <b-button href="#" variant="primary">예약하러 가기</b-button>
    </b-card>
    <b-card
      title="Card Title"
      img-src="https://picsum.photos/600/300/?image=25"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
      id="card2"
    >

      <b-card-text>
        Some quick example text to build on the card title and make up the bulk of the card's content.
      </b-card-text>

      <b-button href="#" variant="primary">예약하러 가기</b-button>
    </b-card>
    </b-card-group>
</div>
</template>

<script>
export default {
  name: 'bespin',
  data(){
    return{};
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#card-g{
  margin :50px;
}
#card1,#card2{ 
  margin:15px;
  background-color: #FFFDFD;
}
#container{
  padding:50px;
}
#carousel-1{
  padding :50px;
}
#cardtxt{
  font-size:14px;
}
</style>
