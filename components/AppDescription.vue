<template>
  <div class="w-60">
    <span class="font-bold mb-1 line-22">Whether you are a seasoned user of Adobe Photoshop CC, or completely unaware of
      what an
      image made up of pixels is, this course will enable you to become true professionals in photo editing, montage and
      photographic development of digital images.</span><br>

    I have spent most of my professional experience dealing with software tools for the design and creation of digital
    images, and since its inception I have followed the development and evolution of Adobe Photoshop first as an
    operator of photo editing stations dedicated to it, then as a consultant for prepress and photography companies, and
    finally for 16 years as presales manager at the Italian headquarters of Adobe Systems. This necessary premise to say
    that I have gained a profound knowledge of this wonderful tool, such as to allow me to understand, in the vastness
    of the functions and tools it offers, what is really useful and necessary to know compared to what represents
    something of rare utility.<br>

    <span v-if="textExpanded" class="font-bold mb-1 mt-1 line-22">This course condenses all my experience gained up to
      now in the knowledge
      of Adobe
      Photoshop, and aims to convey to you, in the clear and simple way that has always characterized me, what you
      absolutely need to know about this tool to become true professionals of the modern digital image processing,
      nothing more and nothing less: only the essentials!</span><br>

    <span v-if="textExpanded" class="font-bold">Novelty!</span> The course has been updated with a section dedicated to
    pictorial brushes
    (14 lessons for more than two
    hours of video course) aimed at all digital artists who want to use Photoshop CC for their works.
  </div>
  <div v-if="textExpanded" class="pt-5">
    <h2>Who this course is for:</h2>
    <ul>
      <li>The beginner who wants to learn digital image processing from scratch</li>
      <li>The expert who wants to refine their techniques</li>
      <li>Anyone who wants to professionally master Adobe Photoshop and its most important features</li>
    </ul>
  </div>
  <div v-if="textExpanded">
    <button @click="textExpand()"
      class="d-flex align-items-center color-strongPurple border-none pointer font-bold bg-white">Show less<svg
        fill="#5624d0" height="14px" width="14px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 330 330" xml:space="preserve" style="margin-left: 4px;">
        <path id="XMLID_224_"
          d="M325.606,229.393l-150.004-150C172.79,76.58,168.974,75,164.996,75c-3.979,0-7.794,1.581-10.607,4.394
	l-149.996,150c-5.858,5.858-5.858,15.355,0,21.213c5.857,5.857,15.355,5.858,21.213,0l139.39-139.393l139.397,139.393
	C307.322,253.536,311.161,255,315,255c3.839,0,7.678-1.464,10.607-4.394C331.464,244.748,331.464,235.251,325.606,229.393z" />
      </svg></button>
  </div>
  <div v-if="!textExpanded">
    <button @click="textExpand()"
      class="d-flex align-items-center color-strongPurple border-none pointer font-bold bg-white mt-3">Show more<svg
        fill="#5624d0" height="14px" width="14px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 330 330" xml:space="preserve" style="margin-left: 4px;">
        <path id="XMLID_225_" d="M325.607,79.393c-5.857-5.857-15.355-5.858-21.213,0.001l-139.39,139.393L25.607,79.393
	c-5.857-5.857-15.355-5.858-21.213,0.001c-5.858,5.858-5.858,15.355,0,21.213l150.004,150c2.813,2.813,6.628,4.393,10.606,4.393
	s7.794-1.581,10.606-4.394l149.996-150C331.465,94.749,331.465,85.251,325.607,79.393z" />
      </svg></button>
  </div>

</template>

<style lang="postcss">
.font-bold {
  font-weight: bold;
}

.w-60 {
  width: 60%;
}

.mb-1 {
  margin-bottom: 4px;
}

.pt-5 {
  padding-top: 20px;
}

.mt-1 {
  margin-top: 4px;
}

.pointer {
  cursor: pointer;
}

.color-strongPurple {
  color: #5624d0;
}

.bg-white {
  background-color: white;
}

.mt-3 {
  margin-top: 15px;
}
</style>

<script lang="ts" setup>
import { defineComponent, PropType, ref } from 'vue'
const textExpanded = ref<boolean>(true);

function textExpand() {
  textExpanded.value = !textExpanded.value;
}

</script>