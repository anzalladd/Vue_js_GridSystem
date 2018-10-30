<template>
   <div class="container">
       <header>
           <h1>This a Header</h1>
       </header>
       <div class="sidebar">
           <h1>This is a sidebar</h1>
       </div>
       <main>
           <div class="card">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusamus, eligendi.</div>
           <div class="card">Accusamus ab maxime inventore quos totam vero similique autem ratione!</div>
           <div class="card">Atque neque pariatur cumque maxime illum alias qui facere sed.</div>
           <div class="card">Voluptas, architecto rerum animi facere minima facilis inventore voluptate enim.</div>
           <div class="card">Reprehenderit praesentium tempore eos sed non natus saepe. In, facere!</div>
           <div class="card">Corporis animi consequatur sed magni incidunt? Molestias inventore quaerat perspiciatis.</div>
           <div class="card">Ad libero amet debitis consectetur, quisquam dignissimos excepturi ratione aliquam?</div>
           <div class="card">Consectetur totam, laborum delectus doloribus voluptatem sunt! Exercitationem, deserunt expedita.</div>
           <div class="card">Minima hic corporis illum maxime sequi odio obcaecati? Soluta, excepturi?</div>
       </main>
            <div class="best">
                <h1>Top Picture</h1>
              <img src="../assets/rumah.jpeg" alt="">
            </div>
       
       <footer>
           <h1>This is a footer</h1>
       </footer>
   </div>
</template>
<script>
export default {
    name: 'Content',
}
</script>
<style lang="scss">

    .container{
        width: 100%;
        display: grid;
        margin: 0 auto;
        grid-gap: 20px;
        grid-template-columns: 10% 45% 45%;
        grid-template-rows: repeat(3,auto);
        
        
        div{
            background: lightblue;
            padding: 20px;
            
            &:nth-child(odd){
                background:limegreen;
            }

        }
        header,footer{
            grid-column: 1/4;
            padding: 20px;
            background:lightcoral;
            color: white;
            
        }
        main{
            display: grid;
            grid-template-columns: repeat(3,1fr);
            grid-template-rows: repeat(3,1fr);
            grid-gap: 20px;
            
            div{
                padding: 20px;
            }
            div:first-child{
                grid-column: 1/ span 2;
                grid-row: 1/ span 2;
            }
            
        }
        .best{
            display: flex;
        img{
        
            align-self: center;
            margin-top: 40px;
        }
        h1{
            align-self: flex-start;
            position: relative;
            left: 350px;
            color: black;
        }
            
        }
  
        
    

    }
    
</style>
