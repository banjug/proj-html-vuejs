<template>
  <div id="app">
    <MyHeader
    :headerNavSections="headerNavSections"
    />
    <MyMain/>
    <MyFooter
    :exploreLinks="exploreLinks"
    :informationLinks="informationLinks"
    />
    <div class="top-btn" @click="scrollToTop" v-if="scroll > 800"><i class="fas fa-arrow-up"></i></div>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  },
  data() {
    return {
      headerNavSections: [
        'Home',
        'Pages',
        'Courses',
        'Features',
        'Blog',
        'Shop',
      ],
      footerLinks: [
        {
          url: '#',
          name: 'Start Here',
          section: 'explore'
        },
        {
          url: '#',
          name: 'Blog',
          section: 'explore'
        },
        {
          url: '#',
          name: 'About Us',
          section: 'explore'
        },
        {
          url: '#',
          name: 'Success Story',
          section: 'explore'
        },
        {
          url: '#',
          name: 'Courses',
          section: 'explore'
        },
        {
          url: '#',
          name: 'Blog',
          section: 'explore'
        },
        {
          url: '#',
          name: 'Contact Us',
          section: 'explore'
        },
        {
          url: '#',
          name: 'Membership',
          section: 'information'
        },
        {
          url: '#',
          name: 'Purchase Guide',
          section: 'information'
        },
        {
          url: '#',
          name: 'Privacy Policy',
          section: 'information'
        },
        {
          url: '#',
          name: 'Terms of Service',
          section: 'information'
        },
      ],
      scroll: 0
    }
  },  
  computed: {
      exploreLinks() {
          return this.footerLinks.filter(x => x.section === 'explore')
      },
      informationLinks() {
          return this.footerLinks.filter(x => x.section === 'information')
      }
  },
  methods: {
    scrollToTop() {
      window.scrollTo(0,0)
    },
    getScroll() {
      this.scroll = window.scrollY;
    }
  },
  created() {
    window.addEventListener('scroll', this.getScroll)
  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');
  @import '~@fortawesome/fontawesome-free/css/all.min.css';
  *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
#app {
  font-family: 'Roboto', sans-serif;
  width: 100%;
  .top-btn {
    width: 80px;
    aspect-ratio: 1;
    background: #20ad96;
    position: fixed;
    bottom: 10%;
    right: 5%;
    border-radius: 100%;
    cursor: pointer;
    .fa-arrow-up {
      color: #ffffff;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 1.6rem;
    }
  }
}
</style>
