<template>
  <div class="back-img">

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
     <!--ImmagineDc-->
     <div class="footer-image container">
         
     </div>
     <!--navigazione sotto-->


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
//Footer
.footer {
   display: flex;
   justify-content: flex-start; 
}
/*Back img*/
.back-img {
   background-image: url(../assets/img/footer-bg.jpg);
   background-repeat: no-repeat;
   background-position: center;
   height: 100%;
   background-size: cover;
   position: relative;
}
// lista
ul {
   list-style: none;
   margin: 20px; 
  // text-transform: uppercase;
}
li {
   a {
       text-decoration: none;
       color: #959595;
      }
      padding:  5px;    
}
h2 {
  color: #fff;
  margin: 20px;
}
.footer-image {
   background-image:url(../assets/img/dc-logo-bg.png);
   background-repeat: no-repeat;
   background-position: right;
   width: 100%;
   height: 400px;
   position: absolute;
   top: 0;
   right: 0;
}

</style>