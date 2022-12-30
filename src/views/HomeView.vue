<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
<!-- Head of the site -->
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-grey">Hello</h1>
              <h1 class="text-white">I'm Greg</h1>
              <span class="text-grey">IT Project manager</span><br />
              <v-btn title dark class="text-yellow mt-8" variant="outlined">Contact</v-btn>


            </div>
          </v-col>


          <v-col cols="2">
            <div
              style="position: absolute ; z-index: 9999; bottom: 0; margin-left: auto;margin-right: auto; left: 0; right: 0; text-align: center ;">
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>




          <v-col cols="5">
            <div style="position: relative;z-index: 9999;" class="mt-16">
              <v-img src="1.png" contain max-height="350" style="transform: skew(0deg, -6deg);"></v-img>

            </div>

          </v-col>
        </v-row>

      </div>

<!-- Section About me du site -->

      <v-col cols="12" class="mt-16" id="contact">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="1.png" max-height="200"></v-img>

              </div>

            </v-col>

            <v-col cols="12" sm="6">
              <h5 class="mt-16" style="margin-bottom: 15px;">About me</h5>
              <div style="width: 120px;">

              </div>
              <h4 class="mt-n4">Seasonnals project manager</h4>
              <p class="text-grey">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit quos aperiam
                dignissimos sed sunt illo? Dignissimos, maiores quasi facilis molestias repellendus voluptates, at
                molestiae natus iste provident deserunt atque. Quod.</p><br />
              <p class="text-grey">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit quos aperiam
                dignissimos sed sunt illo? Dignissimos, maiores quasi facilis molestias repellendus voluptates, at
                molestiae natus iste provident deserunt atque. Quod.</p>

            </v-col>
          </v-row>
        </div>
      </v-col>

<!-- Section portfolio du site -->
    </v-container>
  </v-app>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import NavBar from '@/components/NavBar.vue'

export default defineComponent({
  name: 'HomeView',

  components: {
    NavBar,
  },
});
</script>
<style scoped>
.v-container {
  padding: 16px 0;
}

.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  widows: 100%;
  color: white;
}

.head:before {

  content: " ";
  position: absolute;
  top: -3px;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}

.head:after {

  content: " ";
  position: absolute;
  top: -3px;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}



.egg {

  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 356px;
  height: 300px;
  background-color: #fbdf7e;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
</style>
