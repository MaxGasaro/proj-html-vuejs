<template>
  <div id="app">
    <MyHeader :itemsNav="itemsNav"/>
    <MyMain/>
    <MyFooter :quickLinks="quickLinks" :resources="resources"/>
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
    MyFooter
  },
  data() {
    return {
      itemsNav: [
        {
          text: 'Home',
          url: '#home'
        },
        {
          text: 'About',
          url: '#about'
        },
        {
          text: 'Services',
          url: '#services'
        },
        {
          text: 'Blog',
          url: '#blog'
        },
        {
          text: 'Contact',
          url: '#contact'
        },
        {
          text: 'Portfolio',
          url: '#portfolio'
        },
      ],
      quickLinks: [
        {
          text: 'Quick Links',
          url: '#quicklinks'
        },
        {
          text: 'Services',
          url: '#services'
        },
        {
          text: 'Contact',
          url: '#contact'
        },
        {
          text: 'Blog',
          url: '#blog'
        }
      ],
      resources: [
        {
          text: 'Resource',
          url: '#resource'
        },
        {
          text: 'Art Design',
          url: '#artdesign'
        },
        {
          text: 'Computer',
          url: '#computer'
        },
        {
          text: 'IT News',
          url: '#itNews'
        },
        {
          text: 'Networking',
          url: '#Networking'
        },
        {
          text: 'Web Security',
          url: '#webSecurity'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
</style>
