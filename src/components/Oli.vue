<template>
  <div>
    <button>GET</button>
    <button>POST</button>
    <button>PATCH</button>
    <button>DELETE</button>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    GET: function(url = "") {
      fetch(url, {
        METHOD: "GET"
      })
        .then(response => response.json())
        .then(data => console.log(data));
    },
    POST: function() {},
    PATCH: function() {},
    DELETE: function() {}
  }
};
</script>

<style lang="scss" scoped>
</style>