<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/profile">Profile</router-link> |
      <router-link to="/explore">Explore</router-link> |
      <router-link to="/direct">Direct Message</router-link>
    </div>
    <router-view />
  </div>
</template>
