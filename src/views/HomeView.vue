<template>
    <home-top></home-top> 
    <about-body></about-body>
    <ingredients-body></ingredients-body>
    <menu-body></menu-body>
    <reviews-body></reviews-body>
    <reservationsBody>
    </reservationsBody>
    <home-footer></home-footer>
    <router-view/>
  </template>
  <script>
      import homeTop from "@/components/template/homeTop.vue";
      import aboutBody from "@/components/template/aboutBody.vue";
      import ingredientsBody from "@/components/template/ingredientsBody.vue";
      import menuBody from "@/components/template/menuBody.vue";
      import reviewsBody from "@/components/template/reviewsBody.vue";
      import reservationsBody from "@/components/template/reservationsBody.vue";
      import homeFooter from "@/components/template/homeFooter.vue";
      export default{
        name: "HomeView",
        setup(){  
        },
        components:{
          homeTop,
          aboutBody,
          ingredientsBody,
          menuBody,
          reviewsBody,
          reservationsBody,
          homeFooter
        }
      }
</script>