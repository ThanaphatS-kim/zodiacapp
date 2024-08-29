<template lang="">
    <div>
        <ul>
            <li><a class="active" href="#home">Home</a></li>
            <li><a href="#news">News</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="#about">About</a></li>
            <li class="button"><button>Login</button></li>
        </ul>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Kanit&display=swap');
*{
    box-sizing: border-box;
    font-family: 'Kanit', sans-serif;
    text-align: center;
}
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
  width: 100%;
}
li {
  float: left;
}
li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}
li a:hover {
  background-color: #111;
}
.button button {
  position: absolute;
  right: 2rem;
  top: 1.2rem;
  font-size: 14px;
  width: 70px;
  height: 30px;
  background-color: aliceblue;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  transition: 0.3s;
}

.button button:hover {
  background-color: gray;
  color: aliceblue;
}
</style>