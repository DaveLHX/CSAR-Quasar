<template>
<section>
  <!-- Do you need Material Icons? -->
  <link href="https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900|Material+Icons" rel="stylesheet" type="text/css">

  <!-- Do you need Fontawesome? -->
  <link href="https://use.fontawesome.com/releases/v5.0.13/css/all.css" rel="stylesheet">

  <!-- Do you need Ionicons? -->
  <link href="https://cdn.jsdelivr.net/npm/ionicons@^4.0.0/dist/css/ionicons.min.css" rel="stylesheet">

  <!-- Do you need MDI? -->
  <link href="https://cdn.jsdelivr.net/npm/@mdi/font@^2.0.0/css/materialdesignicons.min.css" rel="stylesheet">

  <!-- Do you need all animations? -->
  <link href="https://cdn.jsdelivr.net/npm/animate.css@^3.5.2/animate.min.css" rel="stylesheet">


  <!--
    Finally, add Quasar's CSS:
    Replace version below (0.17.8) with your desired version of Quasar.
    Replace ".mat" with ".ios" for the iOS theme.
    Add ".rtl" for the RTL support (example: quasar.mat.rtl.min.css).
  -->

  <!-- Do you want IE support? Replace "0.17.8" with your desired Quasar version -->
  <script src="https://cdn.jsdelivr.net/npm/quasar-framework@0.17.8/dist/umd/quasar.ie.polyfills.umd.min.js"></script>



  <!--
    Add Quasar's JS:
    Replace version below (0.17.8) with your desired version of Quasar.
    Replace ".mat" with ".ios" for the iOS theme.
  -->
  <script src="https://cdn.jsdelivr.net/npm/quasar-framework@0.17.8/dist/umd/quasar.mat.umd.min.js"></script>

 <temp-component></temp-component>

</section>
   

</template>

<script>
import "@/styles/quasar.styl";

import TempComponent from "@/components/TempComponent";
export default {
  name: "PageAbout",
  components: { TempComponent }
};
</script>