<template>
  <h1>Instructor</h1>
  <span class="color-strongPurple border-bottom font-bold text-25 border-purple-color">Alberto Comper</span>
  <div class="text-lightblack text-18">Digital Media Evangerlist</div>
  <div class="d-flex">
    <img src="/img/image.jpg" width="112px" height="112px" alt="" class="border-half-radius">
    <div class="pl-5 pb-1">
      <div class="d-flex align-items-center">
        <img src="/img/black-star.png" width="20px" height="20px" alt="">
        <div class="pl-3 text-21">4.7 Instructor Rating</div>
      </div>
      <div class="d-flex align-items-center">
        <img src="/img/review-icon.png" width="20px" height="20px" alt="">
        <div class="pl-3 text-21">11,605 Reviews</div>
      </div>
      <div class="d-flex align-items-center">
        <svg class="svg-icon"
          style="width: 20px; height: 20px;vertical-align: middle;fill: currentColor;overflow: hidden;"
          viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M512 597.994667q108.010667 0 225.002667 46.997333t116.992 123.008l0 85.994667-684.010667 0 0-85.994667q0-76.010667 116.992-123.008t225.002667-46.997333zM512 512q-69.994667 0-120-50.005333t-50.005333-120 50.005333-121.002667 120-51.008 120 51.008 50.005333 121.002667-50.005333 120-120 50.005333z" />
        </svg>
        <div class="pl-3 text-21">29,067 students</div>
      </div>
      <div class="d-flex align-items-center">
        <img src="/img/play-icon.png" width="20px" height="20px" alt="">
        <div class="pl-3 text-21">15 Courses</div>
      </div>
    </div>
  </div>
  <div class="w-60 pt-4">
    Entusiasta di tecnologia ed arti grafiche sin da ragazzo, ho avuto la possibilità di esprimere al meglio queste
    passioni nel mondo del lavoro cavalcando sin dalle origini l'onda della rivoluzione digitale nella comunicazione
    visiva, sviluppando al contempo capacità nella progettazione grafica, illustrativa e di digital imaging, e profonde
    competenze nell'uso delle tecnologie software correlate. Tali conoscenze, unite ad una spiccata capacità
    comunicativa, mi hanno portato a collaborare con i maggiori vendors nel settore del Digital Media sul versante
    marketing, vendite, consulenza e formazione. “Se non lo sai spiegare in maniera semplice, <span
      v-if="textExpanded">non lo hai capito
      abbastanza bene”: questa frase di Albert Einstein rappresenta il mio mantra, che cerco di applicare costantemente
      nello sviluppo dei miei corsi, offrendo competenza unita ad un linguaggio semplice e comprensibile per
      chiunque.</span>
  </div>
  <div v-if="textExpanded" style="margin-left: -7px; padding-top: 12px;">
    <button @click="textExpand()"
      class="d-flex align-items-center color-strongPurple border-none pointer font-bold bg-white text-16">Show less<svg
        fill="#5624d0" height="14px" width="14px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 330 330" xml:space="preserve" style="margin-left: 4px;">
        <path id="XMLID_224_"
          d="M325.606,229.393l-150.004-150C172.79,76.58,168.974,75,164.996,75c-3.979,0-7.794,1.581-10.607,4.394
	l-149.996,150c-5.858,5.858-5.858,15.355,0,21.213c5.857,5.857,15.355,5.858,21.213,0l139.39-139.393l139.397,139.393
	C307.322,253.536,311.161,255,315,255c3.839,0,7.678-1.464,10.607-4.394C331.464,244.748,331.464,235.251,325.606,229.393z" />
      </svg></button>
  </div>
  <div v-if="!textExpanded" style="margin-left: -7px;">
    <button @click="textExpand()"
      class="d-flex align-items-center color-strongPurple border-none pointer font-bold bg-white mt-3 text-16">Show
      more<svg fill="#5624d0" height="14px" width="14px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 330 330" xml:space="preserve" style="margin-left: 4px;">
        <path id="XMLID_225_" d="M325.607,79.393c-5.857-5.857-15.355-5.858-21.213,0.001l-139.39,139.393L25.607,79.393
	c-5.857-5.857-15.355-5.858-21.213,0.001c-5.858,5.858-5.858,15.355,0,21.213l150.004,150c2.813,2.813,6.628,4.393,10.606,4.393
	s7.794-1.581,10.606-4.394l149.996-150C331.465,94.749,331.465,85.251,325.607,79.393z" />
      </svg></button>
  </div>
</template>

<style lang="postcss">
.text-lightblack {
  color: #6a6f73;
}

.text-25 {
  font-size: 25px;
}

.border-purple-color {
  border-color: #5624d0;
}

.text-18 {
  font-size: 18px;
  line-height: 37px;
}

.pb-1 {
  padding-bottom: 4px;
}

.pl-3 {
  padding-left: 12px;
}

.text-21 {
  font-size: 21px;
  color: #1c1d1f;

}

.text-16 {
  font-size: 16px;
}
</style>

<script lang="ts" setup>
import { defineComponent, PropType, ref } from 'vue'
const textExpanded = ref<boolean>(true);

function textExpand() {
  textExpanded.value = !textExpanded.value;
}

</script>