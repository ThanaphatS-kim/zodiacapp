<template lang="">
    <div>
        <div class="card1">
            <img :src="image" alt="name" style="max-width: 550px; width:100%">
              <div class="container">
                <p><a>NAME : <b>{{ name }}</b></a></p>
                <p><a> : {{ somesay }}</a></p>
              </div>
            </div>
    </div>
</template>

<script>
export default {
    props: ['name','image','somesay']
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Kanit&display=swap');
*{
    box-sizing: border-box;
    font-family: 'Kanit', sans-serif;
    text-align: center;
}
.card1 , .card2 {
  margin-left: auto;
  margin-right: auto;
  display: block;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  max-width: 900px;
  width: 100%;
  padding-top: 10px;
  margin-bottom: 10px;
}
.card1:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}
.card2:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}
.container {
  padding: 2px 16px;
  padding-bottom: 10px;
}
</style>