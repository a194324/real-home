<template>
  <nav class="navbar navbar-expand-lg navbar-light p-0 ">
    <div class="container">
      <a class="navbar-brand logo" href="/"><img src="../assets/images/icons/logo.png" alt="logo" /></a>
      <div class="collapse collapse-fontsize navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-lg-0">
          <li class="nav-item menu-link" v-for="(menu, index) in headerMenuList" :key="index">
            <router-link
            class="nav-link active" aria-current="page"
            :to="menu.path">
              {{ menu.name }}
            </router-link>
          </li>
        </ul>
        <div class="icons">
          <a href="https://www.facebook.com/" target="_blank"><img src="../assets/images/icons/facebook.png" alt="" /></a>
          <a href="https://www.pinterest.ru/" target="_blank"><img src="../assets/images/icons/pinteres.png" alt="" /></a>
          <a href="https://www.instagram.com/" target="_blank"><img src="../assets/images/icons/instagr.png" alt="" /></a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import  {menuList} from '../constants/menuLinks'
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  data() {
    return {
      headerMenuList: menuList,
    }
  },
}
</script>

<style lang="scss">
@import '../assets/layouts/index';

.navbar {
  height: 90px;
}

.navbar-nav {
  height: 90px;
}

.logo {
  padding-right: 180px;
}

.collapse-fontsize {
  font-size: 18px;
}

.menu-link {
  padding: 25px 30px;

  &:hover {
    background: grey;
  }
}

.icons {
  a {
    width: 20px;
    height: 20px;
    text-align: center;
    border: 1px solid grey;
    border-radius: 50%;
    margin-right: 7px;
    display: inline-block;
  }
}
</style>