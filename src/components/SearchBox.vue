<template>
  <div class="card-form">
    <h1>Book Review Search</h1>
    <div class="card-input">
      <input
        type="text"
        class="card-input__input"
        placeholder="Search Term"
        v-model="searchTerm"
      />
      <button class="card-form__button" @click="submitSearch">Search</button>

    </div>
  </div>
</template>

<script>

export default {
  name: "SearchBox",
  components: {},
  data() {
    return {
      searchTerm: "",
    };
  },
  methods: {
    submitSearch() {
      this.$emit("search", this.searchTerm);
    },
  },
};
</script>

<style>
</style>
