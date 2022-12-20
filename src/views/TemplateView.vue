<template>
  <div class="body">
    <header>
      <navbar-component />
    </header>
    <body>
      <slot></slot>
    </body>
    <footer></footer>
  </div>
</template>

<script>
import NavbarComponent from "@/components/NavbarComponent";
export default {
  name: "TemplateView",
  components: {
    NavbarComponent,
  },
};
</script>

<style scoped></style>
