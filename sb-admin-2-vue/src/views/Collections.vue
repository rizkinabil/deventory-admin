<template>
  <div id="page-wrapper">
    <div class="row">
      <div class="col-lg-12">
        <h1 class="page-header">Tables Collections</h1>
      </div>
    </div>

    <div class="row">
      <div class="col-lg-12">
        <div class="panel panel-default">
          <div class="panel-heading">
            <div
              class="btn btn-primary btn-md"
              type="button"
              data-toggle="modal"
              data-target="#AddCollectionModal"
            >
              <font-awesome-icon icon="fa-solid fa-plus" />
            </div>
          </div>
          <div class="panel-body">
            <table
              width="100%"
              class="table table-striped table-bordered table-hover"
              id="dataTables-example"
            >
              <thead>
                <tr>
                  <th>No.</th>
                  <th>Name</th>
                  <th>Action</th>
                </tr>
              </thead>
              <tbody>
                <tr
                  class="odd gradeX"
                  v-for="(item, index) in collections"
                  :key="index"
                >
                  <td>{{ index + 1 }}</td>
                  <td>{{ item.name }}</td>
                  <td>
                    <button
                      type="button"
                      class="btn btn-warning btn-circle btn-sm"
                      data-toggle="modal"
                      data-target="#EditCollectionModal"
                    >
                      <font-awesome-icon icon="fa-solid fa-pen-to-square" />
                    </button>
                    <button
                      type="submit"
                      class="btn btn-danger btn-circle btn-sm"
                    >
                      <font-awesome-icon icon="fa-solid fa-trash" />
                    </button>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
    <!-- modal add collection -->
    <add-collection-modal />

    <!-- modal edit collection -->
    <edit-collection-modal />
  </div>
</template>

<script>
import AddCollectionModal from "../components/collections/addCollections.vue";
import EditCollectionModal from "../components/collections/editCollections.vue";

export default {
  name: "Collections",
  components: { AddCollectionModal, EditCollectionModal },
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      collections: [
        {
          _id: "wasdwasd1234",
          name: "Learning Resource",
        },
        {
          _id: "wasdwasd1234",
          name: "Design Ideas",
        },
        {
          _id: "wasdwasd1234",
          name: "Illustrations",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
