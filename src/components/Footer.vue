<template>
  <div class="footer">
      <div class="footer-container">
          &copy; {{ new Date().getFullYear() }} Rantau Corp | All Right Reserved
      </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    msg: String
  }
}
</script>