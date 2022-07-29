<template>
  <nav>
    <router-link to="/" id="logo-url">
      <img :src="logo" id="logo" :alt="alt" />
    </router-link>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/pedidos">Pedidos</RouterLink>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  props: ["logo", "alt"],
};
</script>

<style>
nav {
  display: flex;
  justify-content: flex-end;
  align-items: center;

  background-color: #222;
  border-bottom: 4px solid #111;

  padding: 15px 50px;
}

#logo-url {
  margin: auto;
  margin-left: 0;
}

#logo {
  width: 40px;
  height: 40px;
}

nav a {
  color: #fcba03;
  text-decoration: none;

  margin: 12px;

  transition: 0.5s;
}

nav a:hover {
  color: #fff;
}
</style>
