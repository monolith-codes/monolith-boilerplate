<template>
  <div class="ProductionMaintenanceWrap">
    <div class="ProductionMaintenance">
      <div class="MaintenanceLogoWrap">
        <Vue3Lottie
          animation-link="https://assets10.lottiefiles.com/packages/lf20_0yfsb3a1.json"
          height="75%"
          width="75%"
          :autoPlay="true"
        />
      </div>

      <div class="MaintenanceWrap">
        <div class="MaintenanceHeadingWrap">
          <h1 class="MaintenanceHeading">MAINTENANCE</h1>
        </div>

        <div class="MaintenanceTextWrap">
          <p class="MaintenanceText">
            Something new is in development...<br />Come back later!
          </p>
        </div>
      </div>

      <div class="MaintenanceBottomLogoWrap">
        <div class="MonolithLogoWrap">
          <div class="MonolithLogo"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Vue3Lottie } from "vue3-lottie";
import "vue3-lottie/dist/style.css";

export default defineComponent({
  name: "ProductionMaintenace",
  props: {},
  mounted() {
    console.log("MOUNTED");
  },
  components: {
    Vue3Lottie,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@media screen and (max-height: 650px) {
  .MaintenanceHeading {
    font-size: 3em !important;
  }
  p {
    font-size: 1em !important;
  }
}

@media screen and (max-width: 550px) {
  h1 {
    font-size: 3em !important;
  }

  p {
    font-size: 1em !important;
  }

  .MaintenanceTextWrap {
    justify-content: flex-start !important;
  }
}

.ProductionMaintenanceWrap {
  display: flex;
  flex-direction: column;
}
.ProductionMaintenance {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  position: fixed;
  height: 100%;
  width: 100%;
  background-color: rgb(75, 74, 74);
}

.MaintenanceLogoWrap {
  justify-content: center;
  align-items: center;
  display: flex;
  width: 100%;
  height: 45%;
}

.MaintenanceLogo {
  width: unset;
  height: 100%;
  aspect-ratio: 1/1;
  background-image: url("../assets/images/mainentance.gif");
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
}

.MaintenanceHeadingWrap {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 50%;
  width: 100%;
}

p {
  font-size: 2em;
}

.MaintenanceWrap {
  display: flex;
  flex-direction: column;
  height: 40%;
  width: 100%;
}

.MaintenanceHeading {
  color: white;
  font-size: 5em;
}

.MaintenanceText {
  text-align: center;
  color: white;
}

.MaintenanceBottomLogoWrap {
  display: flex;
  align-items: flex-end;
  justify-content: center;
  height: 10%;
  width: 100%;
  position: relative;
}

.MonolithLogoWrap {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  width: auto;
  aspect-ratio: 1/1;
}

.MonolithLogo {
  height: 55%;
  width: auto;
  aspect-ratio: 1/1;
  background-image: url("../assets/images/logoweb.webp");
  background-size: contain;
  position: relative;
}

.MaintenanceTextWrap {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 50%;
  width: 100%;
  flex-direction: column;
}
</style>
