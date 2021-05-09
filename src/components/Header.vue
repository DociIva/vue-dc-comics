<template>
    <header>
        <div class="container flex">
             <a href="#">
               <img src="@/assets/img/dc-logo.png" alt="Logo immgine DC">
             </a>
            <nav>
               <ul>
                  <li v-for="(link, index) in links"
                      :key="index"
                  >
                      <a :class="{active: link.act }"
                         :href="link.url"> {{link.label}}</a>
                   </li>
                </ul>
            </nav>
        </div>
        <div class="background">
            
        </div>
    </header>
</template>

<script>
// chiave name: chiave di come abbiamo chiamao il file cioe il nuovo componente
export default {
    name:'Header',
    data() {
        return {
          links: [
              {
                label: 'characters',
                url: '#',
                act: 'true',
              },
              {
                label: 'comics',
                url: '#',
                act: 'false',
              },
              {
                label: 'movies',
                url: '#',
                act: 'false',
              },
              {
                label: 'tv',
                url: '#',
                act: 'false',
              },
              {
                label: 'games',
                url: '#',
                act: 'false',
              },
              {
                label: 'collectibles',
                url: '#',
                act: 'false',
              },
              {
                label: 'videos',
                url: '#',
                act: 'false',
              },
              {
                label: 'fans',
                url: '#',
                act: 'false',
              },
              {
                label: 'news',
                url: '#',
                act: 'false',
              },
              {
                label: 'shop',
                url: '#',
                act: 'false',
              },
            ]
        }
        
    }
}
</script>

<style scoped lang="scss">
// usa modo scss
ul {
    display: flex;
    justify-content: center;
    list-style: none;
    margin: 3rem 1rem;
}

li {
    a {
        padding: 1rem;
        text-decoration: none;
        transition: border-bottom 0.4s;
        color: #464646;
        //&.active,
        &:hover {
           border-bottom: 4px solid #0282f9
        }
      }
      text-transform: uppercase;  
}      
/*img*/
img {
  max-width: 80px;
  height: 60px;
  margin: 1rem;
}
.background {
  background-image: url(../assets/img/jumbotron.jpg);
  height: 400px;
  background-repeat: no-repeat;
}
</style>