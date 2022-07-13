<script setup>
import { RouterView } from 'vue-router'
import Navbar from './components/layouts/Navbar.vue'
</script>

<template>
  <header>
    <Navbar /> 
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style>
 @import './assets/style.css';
@import'../node_modules/bootstrap/dist/css/bootstrap.css';

.button_color {
  color: #75c8ec;
}

.blue_bd_btn {
  border-radius: 6px;
  border: 1px solid #2A68BF;
  color: #fff;
  background-color: #2A68BF;
  padding: 12px 20px;
  width: 200px;
}

.org_bnt {
  background: #FBEEE3;
  box-shadow: 0px 5px 20px rgba(36, 131, 197, 0.2);
  border-radius: 9px;
  color: #2A68BF;
  font-weight: 600;
  font-size: 24px;
  line-height: 29px;
  padding: 10px 20px;
  width: 200px;
}

.yl_btn {
  background: #FFFEF3;
  box-shadow: 0px 5px 20px rgba(36, 131, 197, 0.2);
  border-radius: 9px;
  color: #2A68BF;
  font-weight: 600;
  font-size: 24px;
  line-height: 29px;
  padding: 10px 20px;
  width: 200px;
}

.blue_bg_btn {
  background: #F3FAFF;
  box-shadow: 0px 5px 20px rgba(36, 131, 197, 0.2);
  border-radius: 9px;
  color: #2A68BF;
  font-weight: 600;
  font-size: 24px;
  line-height: 29px;
  padding: 10px 20px;
  width: 200px;
}

.gn_light_bnt {
  background: #F3FFF5;
  box-shadow: 0px 5px 20px rgba(36, 131, 197, 0.2);
  border-radius: 9px;
  color: #2A68BF;
  font-weight: 600;
  font-size: 24px;
  line-height: 29px;
  padding: 10px 20px;
  width: 200px;
}

.blue_btn {
  border-radius: 30px;
  border: 2px solid #75C8EC;
  color: #75C8EC;
  background-color: transparent;
  padding: 10px 20px;
  width: 201px;
  filter: drop-shadow(0px 0px 12px rgba(197, 251, 255, 0.4));
  font-weight: 600;
  font-size: 24px;
  line-height: 29px;
}
</style>
