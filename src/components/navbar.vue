<script setup>

import Nav from 'vue-nav-ui';

</script>

<template>
    <Nav :navLinks="navLinks" :navConfig="navConfig" :btnConfig="btnConfig">
        <img class="img" src="./icons/logos1.vue" alt="" srcset="" />
    </Nav>
</template>

<script>
export default {
  components: {
    Nav,
  },
  setup() {
    const navLinks = ref([
      {
        name: "Home",
        path: "/",
      },
      {
        name: "Category",
        path: "/category",
      },
      {
        name: "Works",
        path: "/works",
      },
      {
        name: "About",
        path: "/about",
      },
      {
        name: "Contact",
        path: "/contact",
      },
    ]);
    const navConfig = ref({
      // nav configs here
    });
    const btnConfig = ref({
      // button configs here
    });
    return { navLinks, btnConfig, navConfig };
  },
};

const navConfig = ref ({
    whitespace: true,
    navBg:"#242526",
    navBorderRadius: "30px",
    linkFont: "Ubuntu",
    linkColor: "yellow",
    responsivePosition: "top" || "bottom",
});
const btnConfig = ref ({
    btnLink: true,
    btnUrl: "",
    btnText: "",
    btnBg: "#12BE26",
    btnTextColor: "white",
    btnBorderWidth: "0",
    btnBorderColor: "transparent",
    btnBorderRadius: "20px",
});
</script>