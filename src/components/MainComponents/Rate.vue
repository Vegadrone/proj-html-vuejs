<template>
  <div class="container">
    <div class="row">
      <div class="col-12 d-flex justify-content-between">
        <RateCard
          class="square-card"
          v-for="(element, index) in rateElements"
          :key="index"
          :percentRate="element.percentRate"
          :rateType="element.rateType"
        />
      </div>
    </div>
  </div>
</template>

<script>
import RateCard from "./RateCard.vue";

export default {
  name: "Rate",

  components: {
    RateCard,
  },

  data: function () {
    return {
      rateElements: [
        {
          percentRate: "95%",
          rateType: "pass rate",
        },
        {
          percentRate: "100%",
          rateType: "referral rate",
        },
        {
          percentRate: "0%",
          rateType: "accident rate",
        },
      ],
    };
  },
};
</script>

<style>
</style>