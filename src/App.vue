<script>
import TheMain from './components/TheMain.vue';
import ThePromotion from './components/ThePromotion.vue';
import TheWatchNetflix from './components/TheWatchNetflix.vue';
import ThePromotionWindow from './components/ThePromotionWindow.vue';
import TheWatchDevices from './components/TheWatchDevices.vue';
import TheProfileForKids from './components/TheProfileForKids.vue';
import TheDownLoadSeries from './components/TheDownLoadSeries.vue';
import TheQuestions from './components/TheQuestions.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  name: "App",
  components: {
    ThePromotion,
    TheMain,
    TheWatchNetflix,
    ThePromotionWindow,
    TheWatchDevices,
    TheProfileForKids,
    TheDownLoadSeries,
    TheQuestions,
    TheFooter
  }
}
</script>

<template>
  <ThePromotionWindow />
  <ThePromotion />
  <TheMain />
  <TheWatchNetflix />
  <TheWatchDevices />
  <TheProfileForKids />
  <TheDownLoadSeries />
  <TheQuestions />
  <TheFooter />
</template>

<style>
</style>
