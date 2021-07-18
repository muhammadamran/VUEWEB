<template>
  <div class="menu-container" :class="{'active': toggle}">
      <div class="menu-overlay"></div>
      <button class="menu-close" @click.prevent="$emit('closeMenu')">
          <img src="/img/examples/close-button-white.svg" >
      </button>
      <ul class="menu">
          <li :class="{'active': $route.name == 'index'}" @click.prevent="$router.push('/');$emit('closeMenu');">
              <a href>Home</a>
          </li>
          <li :class="{'active': $route.name == 'about'}" @click.prevent="$router.push('/about');$emit('closeMenu');">
              <a href>About</a>
          </li>
          <li :class="{'active': $route.name == 'projects'}" @click.prevent="$router.push('/projects');$emit('closeMenu');">
              <a href>Projects</a>
          </li>
          <li :class="{'active': $route.name == 'contact'}" @click.prevent="$router.push('/contact');$emit('closeMenu');">
              <a href>Contact Us</a>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'Sidebar',
  props: {
    msg: String
  }
}
</script>