<script>
import TheMain from '../src/components/TheMain.vue';
import ThePromotion from '../src/components/ThePromotion.vue';
import TheWatchNetflix from '../src/components/TheWatchNetflix.vue';
import ThePromotionWindow from '../src/components/ThePromotionWindow.vue';
import TheWatchDevices from '../src/components/TheWatchDevices.vue';
import TheProfileForKids from '../src/components/TheProfileForKids.vue';
import TheDownLoadSeries from '../src/components/TheDownLoadSeries.vue';
import TheQuestions from '../src/components/TheQuestions.vue';
import TheFooter from '../src/components/TheFooter.vue';

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
