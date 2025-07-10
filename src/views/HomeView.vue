<template>

<header class="text-center py-8 bg-[#3B0A0A]">
  <h1 class="text-2xl md:text-3xl font-semibold text-white tracking-wide uppercase">
    Tarot Yolculuğuna Hoşgeldin
  </h1>

  <p class="text-lg text-white ">Umarım bu yol sana uğur getirir. 💜</p>

  <img src="c:\Users\m\Downloads\indir (2).jpeg" alt="Açıklama" style="display: block; margin: 0 auto; width: 15%;" />

  <p class="text-lg text-white text-center py-8 bg-[#3B0A0A]"> Kartların anlamlarını merak ediyor musun?</p>
<p class="text-lg text-white py-8 bg-[#3B0A0A]"> O zaman Büyük Arkanalar ile başlayalım 🔮</p>

</header>

<template v-for="item, index in cards" :key="index">
 
      <div class="collapse bg-[#3B0A0A] border border-base-300">
        <input type="radio" name="my-accordion-1" />
        <div class="collapse-title font-semibold text-amber-50">{{ item.title }}</div>
        <div class="collapse-content text-sm text-amber-50 ">
          <template v-for="content, index in item.contents" :key="index">
            <p>{{ content }}</p>
          </template>
        </div>
      </div>
    </template>










</template>

<script lang="ts">
export default {
data() {
    return {
      cards: [
        { title: "I - The Magician (Büyücü)", contens: ["Teması: Potansiyel, yaratım, odaklanma.","Dikey: Gücünü kullan, harekete geç, zihinsel odaklanma ve beceri."] },
      ]
    }
  }
}
</script>

<style>
h1 {
  margin-bottom: 20px;
}

</style>
