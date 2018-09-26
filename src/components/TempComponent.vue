<template>
<section>
<h6>===Start of TempComponent.vue</h6>
<q-tabs>
  <!-- Tabs - notice slot="title" -->
  <q-tab default count="5" slot="title" name="tab-1" icon="message" />
  <q-tab disable slot="title" name="tab-2" icon="fingerprint" />
  <q-tab alert slot="title" name="tab-3" icon="account_box" />
  <q-tab slot="title" name="tab-4" icon="accessibility" />
  <q-tab slot="title" name="tab-5" icon="build" />

  <!-- Targets -->
  <q-tab-pane name="tab-1"><q-option-group
  type="radio"
  v-model="group"
  :options="[
    { label: 'Option 1', value: 'op1' },
    { label: 'Option 2', value: 'op2', color: 'secondary' },
    { label: 'Option 3', value: 'op3', color: 'amber' }
  ]"/>  
  {{group}}</q-tab-pane>
  <q-tab-pane name="tab-2"></q-tab-pane>
  <q-tab-pane name="tab-3"> <q-knob  :min="min" v-model="knobValue"
  :max="max"
  color="red"
/> Selected value :{{knobValue}}</q-tab-pane>
  <q-tab-pane name="tab-4"><q-datetime  type="datetime" label="Selected a time"/></q-tab-pane>
  <q-tab-pane name="tab-5"><select v-model="selected">
  <!-- inline object literal -->
  <option v-bind:value="{ number: 123 }">123</option>
</select>
<p>Selected value is {{selected}}</p>
</q-tab-pane>
</q-tabs>
 
<q-btn icon="fas fa-plus-circle" color="primary" label="New item" />
  <h6>===End of TempComponent.vue</h6>
</section>
</template>

<script>
export default {
  name: "TempComponent",
  data() {
    return {
      // `v-model` binded to `group`,
      // which must be a String when using radios
      group: "opt1",
      knobValue: 0,
      selected: [],
      max: 100,
      min: 30
    };
  },
  created() {
    console.log("Created: " + this.name);
  }
};
</script>
