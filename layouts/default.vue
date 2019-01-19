<template>
  <div>
    <nav
      class="navbar header has-shadow is-primary"
      role="navigation"
      aria-label="main navigation">
      <div class="navbar-brand">
        <nuxt-link
          to="songs"
          class="navbar-item">
          <img
            src="~assets/buefy.png"
            alt="Buefy"
            height="28">
        </nuxt-link>
        <nuxt-link 
          v-for="(item, key) of items"
          :key="key" 
          :to="item.to"
          class="navbar-item">
          {{ item.title }}
        </nuxt-link>
        <div class="navbar-burger">
          <span/>
          <span/>
          <span/>
        </div>
      </div>
    </nav>

    <section class="main-content columns">
      <div class="container column is-10">
        <nuxt />
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: 'Songs', to: { name: 'songs' } },
        { title: 'songwriters', to: { name: 'songwriters' } },
        { title: 'mission', to: { name: 'mission' } },
      ]
    }
  }
}
</script>
