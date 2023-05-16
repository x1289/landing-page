<template>
  <div>
    <div id="pricing-view">
      <h1>Plans & Pricing</h1>
      <p>Tiered pricing. Only pay for what you really need. Not sure? Feel free to contact us!</p>
      <hr class="border border-success border-3 opacity-75" />
      <div class="d-flex flex-wrap justify-content-center">
        <PriceTier v-for="(priceTier, index) in priceTiers"
          :key="index"
          :title="priceTier.title"
          :pricePerMonth="priceTier.pricePerMonth"
          :includedPoints="priceTier.includedPoints"
          :active="index === priceTiers.length - 1"
          class="d-inline-flex m-3"
        />
      </div>
      <hr class="w-75 m-auto border border-success border-3 opacity-75" />
    </div>
  </div>
</template>

<script setup>
import PriceTier from "../components/pricing/PriceTier.vue"

const priceTiers = [
  {
    title: "FREE",
    pricePerMonth: "$0",
    includedPoints: ["1000 Requests / mo", "All free endpoints", "1 Request per second", "Non commercial use only", "Attribution required"]
  },
  {
    title: "BASIC",
    pricePerMonth: "$10",
    includedPoints: ["Unlimited API Requests", "All basic endpoints", "10 requests per second", "Commercial use", "Live Support", "No Attribution required"]
  },
  {
    title: "PROFESSIONAL",
    pricePerMonth: "$300",
    includedPoints: ["Unlimited API Requests", "All basic endpoints", "Unlimited requests per second", "Commercial use", "Premium Support", "Advanced filtering", "No Attribution required"]
  }
]
</script>

<style scoped>
#pricing-view {
  margin: auto;
  /* background-color: red; */
  max-width: 900px;
}

@media only screen and (max-width: 500px) {
  #login-view {
    max-width: 100%;
  }
}
</style>