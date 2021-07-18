<template>
  <div>
    <Header />
    <Sidebar />
    <Footer />
  </div>
</template>

<script>

export default {
    name: 'DefaultLayout',
    components: {
      Header: () => import('@/components/Header.vue'),
      Sidebar: () => import('@/components/Sidebar.vue'),
      Footer: () => import('@/components/Footer.vue')
    }
}
</script>

<style>
</style>