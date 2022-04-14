<template>
  <div id="app">
    <Navbar />
    <MerchantPhoto />
    <div class="container mx-auto my-8">
      <Breadcrumb />
      <DetailMerchant/>
    </div>
    <MenuMerchant />
    <div class="list-menu_container">
      <Waiki />
      <Aigo />
      <Chingu />
      <SeeramonIkan />
    </div>
    <Footer />
    <Footer2 />
  </div>
</template>

<script>
import Navbar from './components/Navbar/Navbar.vue'
import Breadcrumb from './components/Breadcrumb/Breadcrumb.vue'
import MerchantPhoto from './components/MerchantPhoto/MerchantPhoto.vue'
import DetailMerchant from './components/DetailMerchant/DetailMerchant.vue'
import MenuMerchant from './components/MenuMerchant/MenuMerchant.vue'
import Waiki from './components/ListMenu/Waiki.vue'
import Aigo from './components/ListMenu/Aigo.vue'
import Chingu from './components/ListMenu/Chingu.vue'
import SeeramonIkan from './components/ListMenu/SeeramonIkan.vue'
import Footer from './components/Footer/Footer.vue'
import Footer2 from './components/Footer/Footer_2.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    MerchantPhoto,
    Breadcrumb,
    DetailMerchant,
    MenuMerchant,
    Waiki,
    Aigo,
    Chingu,
    SeeramonIkan,
    Footer,
    Footer2
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

.list-menu_container{
  padding-top: 72px;
  padding-bottom: 72px;
  background-color: #f7f7f7;
}
</style>
