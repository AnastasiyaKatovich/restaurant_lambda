<template>
    <home-top></home-top> 
    <menu-list></menu-list>
    <home-footer></home-footer>

 
    <router-view/>
    </template>
    
    <script>

      import homeTop from "@/components/template/homeTop.vue";
      import menuList from "@/components/template/menuList.vue";
      import homeFooter from "@/components/template/homeFooter.vue";
      export default{
        name: "MenuView",
        setup(){
            
        },
        components:{
          homeTop,
          menuList,
          homeFooter
        }
      }
    </script>