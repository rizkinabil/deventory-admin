<template>
  <div id="wrapper">
    <!-- Navigation -->
    <nav
      class="navbar navbar-default navbar-static-top"
      role="navigation"
      style="margin-bottom: 0"
    >
      <div class="navbar-header">
        <button
          type="button"
          class="navbar-toggle"
          data-toggle="collapse"
          data-target=".navbar-collapse"
        >
          <span class="sr-only">Toggle navigation</span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
        <a class="navbar-brand" href="index.html">{Dev}entory.</a>
      </div>
      <!-- /.navbar-header -->

      <ul class="nav navbar-top-links navbar-right">
        <li class="dropdown">
          <a class="dropdown-toggle" data-toggle="dropdown" href="#">
            <i class="fa fa-user fa-fw"></i> <i class="fa fa-caret-down"></i>
          </a>
          <ul class="dropdown-menu dropdown-user">
            <li>
              <a href="#"><i class="fa fa-user fa-fw"></i> User Profile</a>
            </li>
            <li>
              <a href="#"><i class="fa fa-gear fa-fw"></i> Settings</a>
            </li>
            <li class="divider"></li>
            <li>
              <a href="login.html"
                ><i class="fa fa-sign-out fa-fw"></i> Logout</a
              >
            </li>
          </ul>
        </li>
      </ul>
      <!-- /.navbar-top-links -->

      <!-- side bar -->
      <div class="navbar-default sidebar" role="navigation">
        <div class="sidebar-nav navbar-collapse">
          <ul class="nav" id="side-menu">
            <li>
              <router-link to="/dashboard">
                <i class="fa fa-dashboard fa-fw"></i> Dashboard
              </router-link>
            </li>

            <li>
              <router-link to="/collections">
                <i class="fa fa-table fa-fw"></i> Collections
              </router-link>
            </li>

            <li>
              <router-link to="/blogs">
                <i class="fa fa-table fa-fw"></i> Blogs
              </router-link>
            </li>

            <li>
              <router-link to="/forms">
                <i class="fa fa-table fa-fw"></i> Forms
              </router-link>
            </li>

            <li>
              <a href="#"
                ><i class="fa fa-files-o fa-fw"></i> Sample Pages<span
                  class="fa arrow"
                ></span
              ></a>
              <ul class="nav nav-second-level">
                <li>
                  <router-link to="/blank"> Blank Page </router-link>
                </li>
                <li>
                  <router-link to="/public/login"> Login Page </router-link>
                </li>
              </ul>
              <!-- /.nav-second-level -->
            </li>
          </ul>
        </div>
        <!-- /.sidebar-collapse -->
      </div>
      <!-- /.navbar-static-side -->
    </nav>

    <router-view />
  </div>
</template>

<script>
export default {
  name: "DefaultLayout",
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
