<template>
  <div class="wrapper">
    <div class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout">
          <div
            class="md-layout-item md-size-33 md-small-size-66 md-xsmall-size-100 md-medium-size-40 mx-auto"
          ></div>
          <div>check your email</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  bodyClass: "login-page",
  data() {
    return {
      firstname: null,
      lastName: null,
      email: null,
      password: null
    };
  },
  props: {
    header: {
      type: String,
      default: require("@/assets/img/profile_city.jpg")
    }
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
    }
  },
  methods: {}
};
</script>

<style lang="css"></style>
