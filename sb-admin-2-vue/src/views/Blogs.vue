<template>
  <div id="page-wrapper">
    <div class="row">
      <div class="col-lg-12">
        <h1 class="page-header">Table Blogs</h1>
      </div>
      <!-- /.col-lg-12 -->
    </div>
    <!-- /.row -->
    <div class="row">
      <div class="col-lg-12">
        <div class="panel panel-default">
          <div class="panel-heading">DataTables Advanced Tables</div>
          <!-- /.panel-heading -->
          <div class="panel-body">
            <table
              width="100%"
              class="table table-striped table-bordered table-hover"
              id="dataTables-example"
            >
              <thead>
                <tr>
                  <th>Rendering engine</th>
                  <th>Browser</th>
                  <th>Platform(s)</th>
                  <th>Engine version</th>
                  <th>CSS grade</th>
                </tr>
              </thead>
              <tbody>
                <tr class="odd gradeX">
                  <td>Trident</td>
                  <td>Internet Explorer 4.0</td>
                  <td>Win 95+</td>
                  <td class="center">4</td>
                  <td class="center">X</td>
                </tr>
                <tr class="even gradeC">
                  <td>Trident</td>
                  <td>Internet Explorer 5.0</td>
                  <td>Win 95+</td>
                  <td class="center">5</td>
                  <td class="center">C</td>
                </tr>
              </tbody>
            </table>
            <!-- /.table-responsive -->
            <div class="well">
              <h4>DataTables Usage Information</h4>
              <p>
                DataTables is a very flexible, advanced tables plugin for
                jQuery. In SB Admin, we are using a specialized version of
                DataTables built for Bootstrap 3. We have also customized the
                table headings to use Font Awesome icons in place of images. For
                complete documentation on DataTables, visit their website at
                <a target="_blank" href="https://datatables.net/"
                  >https://datatables.net/</a
                >.
              </p>
              <a
                class="btn btn-default btn-lg btn-block"
                target="_blank"
                href="https://datatables.net/"
                >View DataTables Documentation</a
              >
            </div>
          </div>
          <!-- /.panel-body -->
        </div>
        <!-- /.panel -->
      </div>
      <!-- /.col-lg-12 -->
    </div>
  </div>
  <!-- /#page-wrapper -->
</template>

<script>
export default {
  name: "Blogs",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
