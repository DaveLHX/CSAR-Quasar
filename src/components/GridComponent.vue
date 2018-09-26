<template>
<section>
    <h6>===Start of grid GridComponent.vue</h6>
      Gets 5000 comments from https://jsonplaceholder.typicode.com/comments
<q-table
    title="Table Title"
    :data="comments"
    :columns="columns"
      :filter="filter"
    row-key="id"
  >
  <template slot="top-left" slot-scope="props">
      <q-search
        hide-underline
        color="secondary"
        v-model="filter"
        class="col-6"
      />
    </template>
  </q-table>
     <h6>===End of GridComponent.vue</h6>
</section>

    
</template>




<script>
export default {
  name: "myTestGrid",
  data() {
    return {
      comments: [],
      columns: [
        {
          name: "id",
          required: true,
          label: "id",
          align: "left",
          field: "id",
          sortable: true
          // classes: 'my-class',
          // style: 'width: 500px'
        },
        {
          name: "postId",
          required: true,
          label: "postId",
          align: "left",
          field: "postId",
          sortable: true
          // classes: 'my-class',
          // style: 'width: 500px'
        },

        {
          name: "name",
          required: true,
          label: "name",
          align: "left",
          field: "name",
          sortable: true
          // classes: 'my-class',
          // style: 'width: 500px'
        },

        {
          name: "email",
          required: true,
          label: "email",
          align: "left",
          field: "email",
          sortable: true
          // classes: 'my-class',
          // style: 'width: 500px'
        }
      ],
      filter: ""
    };
  },
  created() {
    fetch("https://jsonplaceholder.typicode.com/comments")
      .then(response => response.json())
      .then(json => {
        this.comments = json;
      });
  }
};
</script>
