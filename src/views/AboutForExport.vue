<template>
<section>
 <h4>Start of AboutForExport.vue</h4>
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
    <link href="https://cdn.jsdelivr.net/npm/quasar-framework@0.17.8/dist/umd/quasar.mat.min.css" rel="stylesheet" type="text/css">


    <!-- Do you want IE support? Replace "0.17.8" with your desired Quasar version -->
    <script src="https://cdn.jsdelivr.net/npm/quasar-framework@0.17.8/dist/umd/quasar.ie.polyfills.umd.min.js"></script>

    <!-- You need Vue too -->
 

    <!--
      Add Quasar's JS:
      Replace version below (0.17.8) with your desired version of Quasar.
      Replace ".mat" with ".ios" for the iOS theme.
    -->
    <script src="https://cdn.jsdelivr.net/npm/quasar-framework@0.17.8/dist/umd/quasar.mat.umd.min.js"></script>

    <!--
      If you want to add a Quasar I18n language pack (other than "en-us").
      Notice "pt-br" in "i18n.pt-br.umd.min.js" for Brazilian Portuguese language pack.
      Replace version below (0.17.8) with your desired version of Quasar.
      Also check final <script> tag below to enable the language
      Language pack list: https://github.com/quasarframework/quasar/tree/dev/i18n
    -->
    <script src="https://cdn.jsdelivr.net/npm/quasar-framework@0.17.8/dist/umd/i18n.pt-br.umd.min.js"></script>

    <!--
      If you want to make Quasar use a specific set of icons (unless you're using Material Icons already).
      Replace version below (0.17.8) with your desired version of Quasar.
      Icon sets list: https://github.com/quasarframework/quasar/tree/dev/icons
    -->
    <script src="https://cdn.jsdelivr.net/npm/quasar-framework@0.17.8/dist/umd/icons.fontawesome.umd.min.js"></script>

<q-page padding>
 <temp-component></temp-component>
<grid-component></grid-component>
</q-page>
<h4>end of AboutForExport.vue</h4>
</section> 
</template>

<script>
//So far this works but there are missing styles when sorting the grid.

import "@/styles/quasar.styl";
// import "quasar-framework/dist/quasar.ie.polyfills";
// import iconSet from "quasar-framework/icons/fontawesome";
// import "quasar-extras/animate";
// import "quasar-extras/roboto-font";
// import "quasar-extras/fontawesome";
// import Quasar from "quasar";

import TempComponent from "@/components/TempComponent";
import GridComponent from "@/components/GridComponent";
export default {
  name: "PageAbout",
  components: { TempComponent, GridComponent },
  created() {
    console.log("demo page created");
  }
};
</script>

