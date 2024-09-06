<script></script>

<template>
  <div class="layout">
    <nav class="breadcrumb">
      <NuxtLink class="link" to="/"> Home </NuxtLink>
      <NuxtLink class="link" to="/categories"> Categories </NuxtLink>
      <NuxtLink class="link" to=""> Category </NuxtLink>
    </nav>
    <slot />
  </div>
</template>

<style scoped lang="scss">
@use "@/assets/styles/colors.scss";

.layout {
  width: 620px;
  margin: 0px auto 50px;
}

.breadcrumb {
  margin-top: 10px;
  margin-bottom: 30px;
  position: relative;
  font-size: 14pt;
  color: colors.$green-dark;
}

.breadcrumb .link {
  height: 28px;
  margin-right: 5px;
  dispay: inline-block;
  color: colors.$green-medium;
}

.breadcrumb .link:hover {
  color: colors.$green-light;
  cursor: pointer;
}
</style>
