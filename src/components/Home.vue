<template>
  <div class="container">
    <h2 class="welcome">Welcome to My Website!</h2>
    <div class="flex-container">
      <h4>My name is Judith Castrejon, nice to meet you</h4>
      <img src="/Users/judithcastrejon/Downloads/Vuejs-portfolio-website/src/assets/IMG_5678_Original.jpeg" alt="Me in the campus gardens" />
      <h4>
        I am a first generation Junior at the University of North Carolina at
        Charlotte. Majoring in Computer Scince with a concentration in Human
        Computer Interaction and this is my first offical website portfolio.
        </h4>
        <h6>
          This is very basic but I plan on adding my projects and connecting all of my social media sites on this website.
        </h6>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
<style scoped>
.flex-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding-top: 4rem;
}
/**Image would just not work for me */
img {
  width: 200px;
  height: 300px;
  margin: 1rem 0;
  border-radius: 5px;
  
}

h4, h6 {
  margin: 0.5rem 0;
  
}

/**Image would just not work for me */
@media(max-width:500px){
  img{
    width:150px;
    height:200px;
    margin: 0 3rem;
  }
  .welcome{
    display: none;
  }
}
</style>
