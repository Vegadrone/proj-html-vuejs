<template>
  <div class="container">
    <div class="row">
      <div class="col-12 d-flex justify-content-between">
        <SquareCard
          class="square-card"
          v-for="(element, index) in rateSecElements"
          :key="index"
          :percentRate="element.percentRate"
          :rateType="element.rateType"
        />
      </div>
    </div>
  </div>
</template>

<script>
import SquareCard from "./SquareCard.vue";

export default {
  name: "Rate",

  components: {
    SquareCard,
  },

  data: function () {
    return {
      rateSecElements: [
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