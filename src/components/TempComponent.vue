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





    <h3>This is the start of a component</h3>
<q-tabs>
  <!-- Tabs - notice slot="title" -->
  <q-tab default count="5" slot="title" name="tab-1" icon="message" />
  <q-tab disable slot="title" name="tab-2" icon="fingerprint" />
  <q-tab alert slot="title" name="tab-3" icon="account_box" />
  <q-tab slot="title" name="tab-4" icon="accessibility" />
  <q-tab slot="title" name="tab-5" icon="build" />

  <!-- Targets -->
  <q-tab-pane name="tab-1">Tab One</q-tab-pane>
  <q-tab-pane name="tab-2">Tab Two</q-tab-pane>
  <q-tab-pane name="tab-3">Tab Three</q-tab-pane>
  <q-tab-pane name="tab-4">Tab Four</q-tab-pane>
  <q-tab-pane name="tab-5">Tab Five</q-tab-pane>
</q-tabs>

<q-option-group
  type="radio"
  v-model="group"
  :options="[
    { label: 'Option 1', value: 'op1' },
    { label: 'Option 2', value: 'op2', color: 'secondary' },
    { label: 'Option 3', value: 'op3', color: 'amber' }
  ]"/>  
<q-datetime v-model="model" type="datetime" label="Selected a time"/>
  <q-knob
  v-model="model"
  :min="min"
  :max="max"
  color="red"
/>
<q-btn icon="fas fa-plus-circle" color="primary" label="New item" />

  <h4>Component END</h4>
</section>
</template>

<script>
import "@/styles/quasar.styl";
// import "quasar-framework/dist/quasar.ie.polyfills";
// import iconSet from "quasar-framework/icons/fontawesome";
// import "quasar-extras/animate";
// import "quasar-extras/roboto-font";
// import "quasar-extras/fontawesome";
// import Quasar from "quasar";

export default {
  name: "TempComponent",
  data() {
    return {
      // `v-model` binded to `group`,
      // which must be a String when using radios
      group: "opt1"
    };
  }
};
</script>
