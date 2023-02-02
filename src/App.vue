<template>
  <div class="container">
    <AppsHeader theTitle="Blogs"/>
    <ButtonLink />
  </div>
</template>
  

<script>
  import AppsHeader from './components/AppsHeader.vue';
  //eslint-disable-next-line
  import ButtonLink from './components/ButtonLink.vue';

  export default{
    name: 'App',
    components: {
      AppsHeader,
      ButtonLink
    }
  }
</script>

  
  <style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap');
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  .box {
    background-color: lightblue;
    border: 1px solid blue;
    min-height: 50px;
    font-size: 2rem;
  }

  body {
    font-family: 'Poppins', sans-serif;
    background-color:beige;
  }
  .container {
    max-width: 500px;
    margin: 30px auto;
    overflow: auto;
    min-height: 300px;
    border: 1px solid rgb(226, 193, 45);
    background-color: blanchedalmond;
    padding: 30px;
    border-radius: 5px;
  }
  .btn {
    display: inline-block;
    background: #000;
    color: #fff;
    border: none;
    padding: 10px 20px;
    margin: 5px;
    border-radius: 5px;
    cursor: pointer;
    text-decoration: none;
    font-size: 15px;
    font-family: inherit;
  }
  .btn:focus {
    outline: none;
  }
  .btn:active {
    transform: scale(0.98);
  }
  .btn-block {
    display: block;
    width: 100%;
  }
  </style>
  