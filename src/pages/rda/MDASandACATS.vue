<template>
  <Card>
    <h1 slot="Title">MDAS and ACATS</h1>
    <div slot="MainContent">
      <div class="FundConceptWrapper">
        <figure>
          <img :src="Image" alt="Graphic flow chart" />
        </figure>
      </div>
    </div>
    <div slot="Notes">
      <h1>MDAS AND ACATS</h1>
      <br />
      <p>Army Systems Acquisitions Review Council (ASARC)</p>
    </div>
  </Card>
</template>
<style scoped>
.FundConceptWrapper {
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.FundConceptWrapper > figure {
  max-width: calc(1449px / 2);
}

.FundConceptWrapper > figure > img {
  width: 80%;
  max-width: calc(1449px / 2);
  height: auto;
}
</style>
<script>
import Card from "../../components/Card.vue";

export default {
  components: {
    Card
  },
  name: "MDASandACATS",

  data() {
    return {
      Image: require("@/assets/MDAS_ACATS.png")
    };
  }
};
</script>