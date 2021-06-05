<template>
  <v-app dark>
    <nav>
      <v-toolbar flat>
      <v-toolbar-title>
        Test commerce
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn v-for="item in items" :key="item.title">
          <v-icon>
            {{ item.icon }}
          </v-icon>
          {{ item.title }}
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
    </nav>
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          icon: "mdi-card-search",
          title: '搜尋商品'
        },
        {
          icon: 'mdi-account-circle',
          title: '會員中心',
          to: '/'
        },
        {
          icon: 'mdi-cart',
          title: '購物車'
        }
      ],
    }
  }
}
</script>
