<template>
    <div class="main">
        <div class="header">
            <img src="../assets/Nsu.png" alt="" style="margin:11.5px 30px;">
        </div>
        <div class="banner" align="center">
                <img src="../assets/main.png" alt="" style="display:block;" id="mainimg">
            <el-button type="primary" round id="mybutton" @click="jump()">进入填报</el-button>
        </div>
    </div>
</template>

<script>
export default {
  methods: {
    jump () {
      this.$router.push('/form')
    }
  }
}
</script>

<style>
    * {
        padding: 0;
        margin: 0;
    }
   .main {
       position: relative;
       display: flex;
       align-content: center;
       justify-content: center;
       flex-wrap: wrap;
       height: calc(100vh);
       width: calc(100vw);
       background: url(../assets/bgi.png) no-repeat;
       background-size: 100% 100%;
    }
    .header {
        position: absolute;
        top: 0;
        left: 0;
        height: 60px;
        width: 100%;
        background-color: rgb(38, 66, 141);
    }
    #mybutton {
        background-color: rgb(149, 173, 233);
        border: none;
    }
    #mybutton:hover {
        background-color: rgba(149, 173, 233, 0.637);
        border: none;
    }
    #mybutton:active {
        background-color: rgba(144, 172, 243, 0.815);
        border: none;
    }
    @media screen and (max-width:450px){
        #mainimg {
            width: 320px;
        }
    }
</style>
