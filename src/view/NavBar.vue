<template>
  <div class="flex">
    <router-link to="/">
      <img src="@/assets/images/logo.png" alt="" />
    </router-link>
    <ul class="flex mt-5">
      <li>
        <router-link to="/movies" class="ml-5"> Movies </router-link>
      </li>
      <li>
        <router-link to="/actors" class="ml-5"> Actors </router-link>
      </li>
      <li>
        <router-link
          to="/profile"
          class="ml-5"
          v-if="this.$store.getters.isUserLoggedIn"
        >
          Profile
        </router-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "NavBar",
};
</script>
<style></style>
