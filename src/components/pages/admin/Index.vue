<template>
  <div>
    <div class="admin-new">
      <div class="container">
        <div class>
          <ul class="admin-menu">
            <!-- Links are to sibling routes -->
            <li>
              <router-link to="/admin">View Products</router-link>
            </li>
            <li>
              <router-link to="/admin/new">New Product</router-link>
            </li>
          </ul>
        </div>
        <!-- Outlet for children routes -->
        <router-view></router-view>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "admin",
  data() {
    return {
      msg: "Welcome to admin page"
    };
  }
};
</script>
<style lang="scss">
.admin-menu {
  width: 300px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: flex-start;
  margin: 0;
  padding: 0;
  li {
    width: 100%;
    height: 50px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: #000;
    border-bottom: 1px solid #fff;
    a {
      color: #ffffff;
      text-decoration: none;
    }
  }
}
</style>
