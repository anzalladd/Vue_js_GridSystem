<template>
<div>
    <nav>
        <img src="../assets/logo.png" alt="logo" id="logo">
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
            <li><a href="#">Profile</a></li>
            
        </ul>
    </nav>
    </div>
</template>

<script>
export default {
    name: 'Nav',
    
}
</script>

<style scoped>

nav{
  position: relative;
  width: 100%;
  height: 60px;
  background-color: #fff;
  box-shadow: -1px -7px 20px 0px #888;
}
nav ul{
  position: relative;
  top: 20px;
  margin: 0;
  float: right;
  right: 10%;
}

nav ul li{
  float: left;
  display: block;
  margin: 0px 15px 0px 15px;
}
nav ul li a{
  text-decoration: none;
  color: #888;
  font-family: 'Helvetica', sans-serif;
}
a:hover{
 color: aqua;
}
#logo{
  position: relative;
  float: left;
  height: 50px;
  width: 50px;
  margin: 5px 0 10px 10px;
}
</style>