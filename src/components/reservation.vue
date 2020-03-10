<template>
<div>
    <b-jumbotron >
        <template v-slot:header style="text-align:left;">현대자동차 베뉴</template>
        <template v-slot:lead style="text-align:left;">
      도심주행에 적합한 안정적이고 편안한 주행성능이 특징이다.
진보된 첨단 지능형 주행 안전 기술 및 편의사양을 원한다면 이차를 선택하세요!
    </template>
    <b-card>
  <b-row>
        <img src="@/assets/car1.png" style="max-width: 30rem;" align="top">
      <b-card>
     <b-table stacked :items="items" width="250" height="100"></b-table>
      </b-card>
  <br>
    <b-col md="auto" @submit="onSubmit" v-if="show">
        <p>▲ 픽업 날짜</p>
      <b-calendar  v-model="value"  :min="min" :max="max" @context="onContext" locale="en" ></b-calendar>
    </b-col>
    <b-col md="auto" @submit="onSubmit" v-if="show">
        <p>▲ 반납 날짜</p>
      <b-calendar  v-model="value1"  :min="min" :max="max" @context="onContext" locale="en" ></b-calendar>
    </b-col>
    <b-col>
      <p>Value: <b>'{{ value }}'</b></p>
      <p>Value: <b>'{{ value1 }}'</b></p>
    </b-col>
  </b-row>
  </b-card>

  </b-jumbotron>
  <center>
  <b-button type="submit" variant="primary" href="#">예약하기</b-button>
    <b-button variant="success" to="/">다른 차 보러가기</b-button>
  </center>
  <br>
  <br>
  <br>
  </div>
</template>

<script>
export default {
    name:'reservartion',
    data() {
        const now = new Date()
      const today = new Date(now.getFullYear(), now.getMonth(), now.getDate())
      // 15th two months prior
      const minDate = new Date(today)
      minDate.setMonth(minDate.getMonth())
      minDate.setDate(3)
      // 15th in two months
      const maxDate = new Date(today)
      maxDate.setMonth(maxDate.getMonth())
      maxDate.setDate(16)
      return {
        value: '',
        value1: '',
        min: minDate,
        max: maxDate,
        context: null,
        items: [
         { 차종: '현대자동차 베뉴', 코드: 'CB0001', 가격: '하루 73425원', 색깔: '검은색', 연료:'디젤',연비:'11.3~16.1km'}
        ],
        show: true
      }
    },
    methods: {
        onSubmit(evt) {
        evt.preventDefault()
        alert("예약이 완료되셨습니다!")
      },
      onContext(ctx) {
        this.context = ctx
      },
    }
  }
</script>