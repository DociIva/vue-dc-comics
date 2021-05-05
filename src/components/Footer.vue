<template>
   <div class="container footer">
      <!--lista-->
      
       <nav>
           <h2>DC COMICS</h2>
          <ul>
             <li v-for="(link, index) in linksDcComics" 
              :key="index"
             >
               <a :href="link.url"> {{link.lable}} </a>
               </li>
            </ul>
         </nav>
      
         <nav>
            <h2>DC</h2>
            <ul>
              <li v-for="(links, index) in linkDc" 
                 :key="index"
                 >
               <a :href="links.url"> {{links.lable}} </a>
               </li>
            </ul>
         </nav>
    
         <nav>
            <h2>SITES</h2>
           <ul>
              <li v-for="(link3, index) in linkSites" 
                 :key="index"
                 >
               <a :href="link3.url"> {{link3.lable}} </a>
               </li>
          </ul>
        </nav>
   </div>

</template>

<script>
// chiave : nome di come abbiamo chiamato il componente
export default {
   name:'Footer',
   data() {
      return {
         linksDcComics: [
            {
               lable:'Characters',
               url: '#',
            },
            {
               lable:'Comics',
               url: '#',
            },
            {
               lable:'Movie',
               url: '#',
            },
            {
               lable:'TV',
               url: '#',
            },
            {
               lable:'Games',
               url: '#',
            },
            {
               lable:'Video',
               url: '#',
            },
            {
               lable:'News',
               url: '#',
            },
           
         ],
         linkDc: [
            {
               lable:'Terms Of Use',
               url: '#',
            },
            {
               lable:'Privacy police (New)',
               url: '#',
            },
            {
               lable:'Ad Choices',
               url: '#',
            },
            {
               lable:'Advertising',
               url: '#',
            },
            {
               lable:'Jobs',
               url: '#',
            },
            {
               lable:'Video',
               url: '#',
            },
            {
               lable:'News',
               url: '#',
            },
            {
               lable:'Characters',
               url: '#',
            },
            {
               lable:'Comics',
               url: '#',
            },
            {
               lable:'Shp Help',
               url: '#',
            },
            {
               lable:'Content Us',
               url: '#',
            } 
         ],
         linkSites: [
            {
               lable:'DC',
               url: '#',
            },
            {
               lable:'MAD Magazine',
               url: '#',
            },
            {
               lable:'DC Kids',
               url: '#',
            },
            {
               lable:'DC Universe',
               url: '#',
            },
            {
               lable:'DC Power Visa',
               url: '#',
            },
         ]
      }
   }
}
</script>

<style scoped lang="scss">
ul {
   list-style: none;
   margin: 20px;
}
li {
   a {
       text-decoration: none;
       color: black;
      }
      padding:  5px;
}
.footer {
   display: flex;
   justify-content: flex-start;
   background: lightseagreen;
      
}
h2 {
  color: #fff;
  margin: 20px;
}

</style>