<script>
  let cats = [
  {
  id:'uHKfrz65KSU',
  name:'baby cute cats',
  image: './src/cat1.jpg'
  },
  {
  id:'jHWKtQHXVJg',
  name:'Other Baby cute cats',
  image: './src/cat2.jpg'
  },
  {
  id:'8ZgjNeXXTjU',
  name:'Humans and cats',
  image: './src/cat3.jpg'
  }
  ];
</script>

<div class="container">
<h1>Youtube Cat Videos</h1>

<!--one link for all videos only the 'id' {cat.id} is different-->
<div class="row"> 
  {#each cats as cat,i}
  <div class="column">
  <a target="_blank" href="https://www.youtube.com/watch?v={cat.id}">    
  <div class="name">{cat.name.toUpperCase()}</div>
     <img src="{cat.image}" alt="">   
  </a> 
</div>
  {/each} 
</div>

<div class="row"> 
  {#each cats as cat,i}
  <div class="column">
  <a target="_blank" href="https://www.youtube.com/watch?v={cat.id}">    
  <div class="name">{cat.name.toUpperCase()}</div>
     <img src="{cat.image}" alt="">   
  </a> 
</div>
  {/each} 
</div>

</div>
<hr>
<footer>
  &#169 Copyright 2022
</footer>

<style>
  .container{
    width: 100%;
    margin-left: 20px;
    margin-right: 20px;   
  }
  h1{
    color: grey;
  }
  a{
    font-size: 20px;
    margin-bottom: 20px;
    color: grey;
  }  
  .name{
    margin-bottom: 5px;
    font-size: 18px;
  }
  img{
    margin-left: 10px;
    margin-right: 10px;    
    padding: -1px 1px;
    border: 2px solid grey;
    width: 80%;
    height: auto  ;
    }
  img:hover{
    border: 2px solid white;
  }
  .column{
    float: left;
    width: 30%;
    padding: 5px;   
  }
  .row::after {
    content: "";
    clear: both;
    display: flex;    
  }  
</style>