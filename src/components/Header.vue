<template>
  <header>

    <img src="../assets/img/dc-logo.png" alt="">
    
    <ul>
      <li v-for="(menu, index) in menuList" :key="index">
        <a href="#">{{ menu.name }}</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{
      menuList:[
        {
          name: 'Characters',
          url: '/',
          active:'false',
        },
        {
          name: 'Comics',
          url: '#',
          active:'true',
        },
        {
          name: 'Movies',
          url: '#',
          active:'false',
        },
        {
          name: 'Tv',
          url: '#',
          active:'false',
        },
        {
          name: 'Games',
          url: '#',
          active:'false',
        },
        {
          name: 'Collectibles',
          url: '#',
          active:'false',
        },
        {
          name: 'Videos',
          url: '#',
          active:'false',
        },
        {
          name: 'Fans',
          url: '#',
          active:'false',
        },
        {
          name: 'News',
          url: '#',
          active:'false',
        },
        {
          name: 'Shop',
          url: '#',
          active:'false',
        },
      ]
    }
  }
}
</script>


<style scoped lang="scss">
@import '../assets/styles/vars.scss';


img {
    width: 100px;
  }

  ul {  
    height: 100%;
    display: flex;
    align-items: center;

    li {      
      font-size: 13px;
      margin: 0 14px;
      text-transform: uppercase;

    }

    a {
      position: relative;
      color: black;

      &:hover {
        position: relative;
        color: inherit;
      }

      &:hover::after{
        content: '';
        position: absolute;
        bottom: -50px;
        left: 50%;
        transform: translateX(-50%);
        height: 3px;
        width: 40px;
        background-color: inherit;
      }
      
    }
  
  }
a:hover {
  color: $brand-color;
}

a:hover::after{
  background-color: $brand-color;
}

</style>
