<template>
  <div id="app" class="flex flex-col h-screen bg-ig-200 text-white">
    
    <Header />
    <Feed />
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header';
import Feed from '@/components/Feed';
import Footer from '@/components/Footer';
export default {
  name: 'App',

  components: {
    Header,
    Feed,
    Footer
  }
}
</script>
