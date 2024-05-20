<script setup>
import ChallengeAsset from "@/components/ChallengeAsset.vue";
</script>

<style scoped>
.app-main{
  background-color:  hsl(0, 0%, 12%);
  width:40%;
  padding:50px 30px;
  font-family: "Inter", sans-serif;
  font-optical-sizing: auto;
}
.app-main-header-image{
  width:100%;
  display:flex;
  place-items: center;
  justify-content:center;
}
.app-main-header-image img{
  width:150px;
  height:100%;
  border-radius:50%;
}
.app-main-header-title{
  text-align: center;
}
.name{
  color:hsl(0, 0%, 100%);
  font-size:28px;
  margin:10px 0;
  font-weight:700;
}
.location{
  color:hsl(75, 94%, 57%);
}
.name-context{
  color:hsl(0, 0%, 100%);
  line-height:2;
  margin:20px 0;
  font-size:14px;
}

.app-btn-main-ctn{
  width:100%;
}
.app-btn{
  background-color:hsl(0, 0%, 20%);
  color:hsl(0, 0%, 100%);
  width: 90%;
  padding:20px 20px;
  text-align:center;
  margin:0 auto;
  font-weight:600;
}
.app-btn:hover{
  background-color:hsl(75, 94%, 57%);
  color: hsl(0, 0%, 0%);
  transition: all .4s;
}
@media screen and (max-width:950px) and (min-width:751px){
  .app-main{
    width:60%;
  }
  .app-main-header-image img{
    width:100px;
  }
  .name{
    font-size:22px;
  }
  .location{
    font-size:14px;
  }
  .name-context{
    font-size:14px;
  }
  .app-btn{
    font-size:16px;
    padding:10px;
  }
}
@media screen and (max-width:750px){
  .app-main{
    width:90%;
  }
  .app-main-header-image img{
    width:100px;
  }
  .name{
    font-size:22px;
  }
  .location{
    font-size:14px;
  }
  .name-context{
    font-size:14px;
  }
  .app-btn{
    font-size:16px;
    padding:10px;
  }
}
</style>


<template>
  <div class="app-main">
    <div class="app-main-content-container">
      <div class="app-main-header">
        <div class="app-main-header-image">
          <img src="/public/avatar-jessica.jpeg" alt="profile-picture">
        </div><br/>
        <div class="app-main-header-title">
          <!--   "" GitHub Frontend Mentor LinkedIn Twitter Instagram -->
          <p class="name">Jessica Randall</p>
          <p class="location">London, United Kingdom</p>
          <p class="name-context"><q>Front-end developer and avid reader.</q> </p>
        </div>
      </div>
      <div class="app-btn-ctn">
        <div class="app-btn">GitHub</div><br/>
        <div class="app-btn">Frontend Mentor</div><br/>
        <div class="app-btn">LinkedIn</div><br/>
        <div class="app-btn">Twitter</div><br>
        <div class="app-btn">Instagram</div>
      </div>
    </div>
    <ChallengeAsset></ChallengeAsset>
  </div>
</template>