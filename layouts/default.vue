<template>
  <a-layout id="components">
    <a-layout-header class="header">
      <img
        src="https://cdn.bimbimbikes.com/media/cache/location_logo/uploads/location/logo/5977aa563d830_LOGO_METAL.jpeg"
        class="logo"
      />
      <a-menu
        theme="dark"
        mode="horizontal"
        :default-selected-keys="['2']"
        :style="{ lineHeight: '64px' }"
      >
        <a-menu-item key="1"
          ><nuxt-link to="/myorders"> My Orders </nuxt-link></a-menu-item
        >
        <a-menu-item key="2"><nuxt-link to="/"> Bikes </nuxt-link></a-menu-item>
      </a-menu>
    </a-layout-header>
    <Nuxt />
  </a-layout>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono:ital@0;1&display=swap');

#components .logo {
  height: 31px;
  margin: 10px 10px;
  float: left;
}
#components {
  background-color: #111;
  font-family: 'Space Mono', monospace;
}
.header {
  background-color: black;
}
.ant-menu {
  background-color: black;
}
</style>
