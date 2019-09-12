<template>
  <div class="bg-orties">
    <section class="section">
      <div class="columns">
        <div class="column is-4 is-offset-4">
          <img src="~/assets/logoagrortie.jpg" />
        </div>
      </div>
    </section>
    <div class="columns">
      <div class="column is-8 is-offset-2">
        <nav
          class="navbar is-dark"
          role="navigation"
          aria-label="main navigation"
        >
          <div class="navbar-brand">
            <a
              role="button"
              class="navbar-burger burger"
              aria-label="menu"
              aria-expanded="false"
              data-target="navbarBasicExample"
              v-bind:class="{ 'is-active': isOpen }"
              @click="isOpen = !isOpen"
            >
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
            </a>
          </div>

          <div
            id="navbarBasicExample"
            class="navbar-menu"
            v-bind:class="{ 'is-active': isOpen }"
          >
            <div class="navbar-start">
              <nuxt-link to="/" class="navbar-item has-text-light">
                Accueil
              </nuxt-link>
              <nuxt-link
                to="/agrortie"
                class="navbar-item has-text-light"
                @click.native="isOpen = !isOpen"
              >
                Qui sommes-nous ?
              </nuxt-link>
              <nuxt-link
                to="/produits"
                class="navbar-item has-text-light"
                @click.native="isOpen = !isOpen"
              >
                Nos produits
              </nuxt-link>
              <nuxt-link
                to="/ortie"
                class="navbar-item has-text-light"
                @click.native="isOpen = !isOpen"
              >
                L'ortie
              </nuxt-link>
              <nuxt-link
                to="/cheval"
                class="navbar-item has-text-light"
                @click.native="isOpen = !isOpen"
              >
                L'ortie et le cheval
              </nuxt-link>
              <div class="navbar-item has-dropdown is-dark is-hoverable">
                <a class="navbar-link has-text-light">Les animaux</a>

                <div class="navbar-dropdown is-dark ">
                  <nuxt-link
                    to="/chien"
                    class="navbar-item has-text-light"
                    @click.native="isOpen = !isOpen"
                  >
                    Les chiens
                  </nuxt-link>
                </div>
              </div>
              <nuxt-link
                to="/contact"
                class="navbar-item has-text-light"
                @click.native="isOpen = !isOpen"
              >
                Contact
              </nuxt-link>
              <nuxt-link
                to="/pub"
                class="navbar-item has-text-light"
                @click.native="isOpen = !isOpen"
              >
                Publicité
              </nuxt-link>
            </div>
          </div>
        </nav>
      </div>
    </div>
    <nuxt />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false
    }
  }
}
</script>
