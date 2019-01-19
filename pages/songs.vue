<template>
  <section class="section">
    <div class="container columns is-mobile">
      <div>
        <div class="card">
          <div class="card-header">
            <p class="cared-header-title has-text-grey">
              Song Title
            </p>
            <br>
            <p class="card-header-title username">UserName</p>
          </div>
          <div class="card-content">
            <div class="content has-text-centered">
              Song description Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iure quo consectetur debitis adipisci soluta vel ipsum hic tenetur. Veritatis, unde!
            </div>
          </div>
          <footer class="card-footer">
            <p>Comment section (input goes here)</p>
          </footer>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import BLogo from '@/components/Logo'

export default {
  name: 'Songs',
  components: { BLogo },
  data() {
    return {
      features: [
        { icon: 'github-circle', title: 'Free', content: `<span>Open source on <a href="https://github.com/buefy/buefy"> GitHub</a></span>` },
        { icon: 'cellphone-link', title: 'Responsive', content: `<span><b class="has-text-grey">Every</b> component is responsive</span>` },
        { icon: 'alert-decagram', title: 'Modern', content: `<span>Built with <a href="https://vuejs.org/">Vue.js</a> and <a href="http://bulma.io/">Bulma</a></span>` },
        { icon: 'arrange-bring-to-front', title: 'Lightweight', content: `<span>No other internal dependency</span>` }
      ]
    }
  }
}
</script>

<style scoped>
.username {
  color: green;
  margin-left: 20px;
}
</style>

