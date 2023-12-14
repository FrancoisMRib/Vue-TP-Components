<template>
  <div>
    <le-header></le-header>
    <badge-list></badge-list>
    <user-info
      :full-name="activeUser.name"
      :info-text="activeUser.description"
      :role="activeUser.role"
    ></user-info>
  </div>
</template>

<script>
import LeHeader from './components/LeHeader.vue';
export default {
  components : {
    'le-header' : LeHeader , 
  } ,
  data() {
    return {
      activeUser: {
        name: 'LOL',
        description: 'admin du site',
        role: 'premium',
      },
    };
  },
};
</script>