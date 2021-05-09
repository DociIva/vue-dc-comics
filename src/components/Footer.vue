<template>
  <div class="back-img">
     
     <div class="bg-footer">
         <div class="img">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <span>DICITALS COMICS</span>
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <span>DICITALS COMICS</span>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <span>DICITALS COMICS</span>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <span>DICITALS COMICS</span>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <span>DICITALS COMICS</span>
         </div>
     </div>
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
     <div class="footer-nav-end flex">
          <div class="accesso">
             <button>Sing Up Now!</button>
          </div>
          <div class="follow-us">
             <span>Follow Us</span>
             <img src="../assets/img/footer-facebook.png" alt="">
              <img src="../assets/img/footer-youtube.png" alt="">
              <img src="../assets/img/footer-pinterest.png" alt="">
              <img src="../assets/img/footer-periscope.png" alt="">
          </div>
     </div>

     
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
.bg-footer {
   width: 100%;
   height: 120px;
   background:#0282f9;
   display: flex;
   justify-content:center;
   align-items: center;
}
.img { 
   display: flex;
   align-items: center;
   flex-basis: max-content;
}
.bg-footer img {
   width: 60px;
}
.bg-footer span {
   font-size: 10px;
   color: #fff;
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
.footer-nav-end {
   background: #303030;
   display: flex;
   justify-content: space-between;
   align-items: center;
}
.accesso {
   display: flex;
   align-items: center;
   padding: 40px;
}
button {
   width: 150px;
   height: 60px;
   padding: 10px;
   border: 3px solid #0282f9;
   background: transparent;
   color: #fff;
   text-transform: uppercase;
   font-size: 1rem;
   transition: background 2s;
}
button:hover {
   background: limegreen;
}
.follow-us {
   display: flex;
   align-items: center;
   padding-right: 80px;
}
span { 
   color: #0282f9;
   padding-left: 10px;
}
img {
   padding: 0 8px;
}
</style>