<template>
  <q-page padding>
   <!--
  16 characters max.
  Notice "count" property (and optional max-length
  to enforce max number of characters)
-->
<q-field
  :count="16"
>
  <q-input type="password" max-length="16" v-model="model" />
</q-field>

<!-- Counting Chips. Notice "count" property -->
<q-field
  count
  icon="fas fa-user-circle"
  helper="Some helper here"
  :label-width="3"
>
  <q-chips-input float-label="Float Label" v-model="model" />
</q-field>

<!-- Counting selected options -->
<q-field
  count
>
  <q-select
    v-model="select"
    :options="[
      {
        label: 'Google',
        icon: 'far fa-envelope-square',
        value: 'goog'
      },
      {
        label: 'Facebook',
        description: 'Enables communication',
        value: 'fb'
      },
      {
        label: 'Twitter',
        secondIcon: 'alarm',
        value: 'twtr'
      }
    ]"
  />
</q-field>


<!-- Single Line Input -->
<q-input v-model="text" />
<q-input v-model="text" stack-label="Stack Label" />
<q-input v-model="text" float-label="Float Label" placeholder="Gigi" />

<!-- Multiple Line Input -->
<q-input
  v-model="area"
  type="textarea"
  float-label="Textarea"
  :max-height="100"
  rows="7"
/><!-- max-height refers to pixels -->
<temp-component></temp-component>

  </q-page>
</template>

<script>
import TempComponent from "@/components/TempComponent";
export default {
  name: "PageAbout",
  components: { TempComponent }
};
</script>
