<template>
  <header>

    <img src="../assets/img/dc-logo.png" alt="">
    
    <ul>
      <li v-for="(menu, index) in menuList" :key="index">
        <a  href="#" class="border-underline"
          @click="focus(menu, index)"
          :class="menu.isActive === true ? 'active' : ''"
        >{{ menu.name }}</a>
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
          isActive: false,
        },
        {
          name: 'Comics',
          url: '#',
          isActive: true,
        },
        {
          name: 'Movies',
          url: '#',
          isActive: false,
        },
        {
          name: 'Tv',
          url: '#',
          isActive: false,
        },
        {
          name: 'Games',
          url: '#',
          isActive: false,
        },
        {
          name: 'Collectibles',
          url: '#',
          isActive: false,
        },
        {
          name: 'Videos',
          url: '#',
          isActive: false,
        },
        {
          name: 'Fans',
          url: '#',
          isActive: false,
        },
        {
          name: 'News',
          url: '#',
          isActive: false,
        },
        {
          name: 'Shop',
          url: '#',
          isActive: false,
        },
      ]
    }
  },
  methods: {
    focus(obj) { //funzione per il click degli li nel header
      console.log(obj);
      if(obj.isActive === true){
        obj.isActive = false
        console.log(obj);
      }else{
        this.menuList.forEach((menu) => {
          menu.isActive = false;
          obj.isActive = true;
        });
      }
    }
  }
}
</script>


<style scoped lang="scss">
@import '../assets/styles/vars.scss';

header { 
  height: 115px;
}

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
        color: $brand-color;
      }
      
      

      
      &.active::after {
        content: '';
        position: absolute;
        bottom: -50px;
        left: 50%;
        transform: translateX(-50%);
        height: 3px;
        width: 100%;
        background-color: $brand-color;
      }
      &:after:hover {
        width: 100%;
      }
    }

    .border-underline::after {
        content: '';
        position: absolute;
        bottom: -50px;
        left: 50%;
        transform: translateX(-50%);
        height: 3px;
        width: 0px;
        background-color: $brand-color;        
    }
    .border-underline:hover::after {
      width: 100%;
      transition: width linear 300ms;
    }
  } //END ul

</style>
