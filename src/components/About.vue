<template>
  <div class="container">
    <!-- page header and little paragraph about myself -->
    <h2>About Me</h2>
    
    <p>
      My Name is Judith Castrejon, I am 21 years old and I have lived in North Carolina for my whole
      life. I am a first-generation college student and am currently a junior, my major is computer science with a
      concentration in Human-Computer Interaction. I am interested in working as a UI/UX designer once I graduate in 2023 and 
      I am currently looking for internships. I am always looking to expand my knowledge, and take initiative, I have learned to use 
      Balsamiq Wireframes and Axure. I love to travel and see new places and have been to the
      Grand Canyon, the Four Corners Monument, New York, and Tennesee. One of my favorite pastimes is
      reading books during my free time and I am currently reading Devil all the time and Crazy Rich Asians and
      the next book on my list is Fahrenheit 451.
    </p>
    <h4>My Skills</h4>
    <!--progress bar to showcase my programming/technical skills  -->
    <!--Based off of https://www.w3schools.com/bootstrap/bootstrap_progressbars.asp -->
    
    <div v-for="skill in skillProgress" :key="skill">
      <h6>{{ skill.title }}</h6>
      <div class="progress">
        <div
          class="progress-bar bg-success"
          role="progressbar"
          :aria-valuenow="`${skill.vNow}`"
          aria-valuemin="0"
          aria-valuemax="100"
          :style="{ width: skill.vStyle }"
        ></div>
      </div>
    </div>
    <br>
    <!-- Tried to place resume as a txt file but I could not figure it out-->
    <h4><u>My Resume:</u></h4>
    <p>
      Judith Castrejon Ortiz   
      <br>                                                                                                   
Charlotte, NC | judithcastrejon4@gmail.com | 980-328-7889 |   LinkedIn  | GitHub 
&nbsp;

<br>
<u><br>EDUCATION</u>
<br>
The University of North Carolina at Charlotte ⎯ Charlotte, NC   &nbsp;  December 2023
<br>
Bachelor of Arts in Computer Science 
<br>
Concentration: Human-Computer interaction
<br>
Overall GPA: 3.54; GPA in Major 3.48 <br>
&nbsp;
&nbsp;
<br>
<u>Course Projects </u> <br>
Nails Divine, Web App Design, and Development     :          &nbsp;   &nbsp;       August 2021- December 2021
<br>
* Web-based application for an individual that promotes their profession, interest, and community project. 
<br>
* Design and develop an interactive web-based application that incorporates HTML, CSS, JavaScript, and jQuery-based interactive elements and access to external data. 
<br>
* Experienced developing a website for a client according to their requirements, incorporating contextual information, and pictures that promote their service. <br>
&nbsp;
&nbsp;


<br>Craps Game, Introduction to Computer Science  II    :     &nbsp;     &nbsp;    August 2020- December 2021
<br>
* Craps dice game, that revolves around rolling two six-sided dice in an attempt to roll a particular number. 
<br>
* A Java-based program that uses printing, loops, variables, if-statements, and switch statements, generating random numbers, using methods and multiple classes. 
<br>
* Wins and losses are determined by rolling the dice and are printed once the first ten rounds are completed. 

<br>
<u><br>Work Experience </u>
<br> Pizza Hut - Wingate, NC     :  &nbsp; &nbsp;  August 2018- August  2020
<br> * Greet customers when they come in, assist them with purchases, and maintain two cash registers.
<br> * Hire and train new employees in customer service, food preparation, and sanitation procedures. 
<br> * Supervising four to six employees preparing food for delivery. Ensuring orders are accurately made, reducing food loss and cost of operations.
<br> * Maintaining inventory, counting items, and placing food orders when items have run out.


<br>
<u><br>CAMPUS INVOLVEMENT </u>
<br>Member, GirlsWhoCode                   : &nbsp;  January 2022- Present 
<br>Member, Latin American Student Organization    : &nbsp;April 2021- Present
<br>Member, Latinx Student Union   :&nbsp;March 2021- Present <br> 



<br>
<u><br>VOLUNTEER EXPERIENCE</u>
<br>
UCPS, Robotics Competition ⎯ Monroe, NC  &nbsp;   October 2021
<br>* Coordinated competition rounds for high school robotics teams.
<br>* Operated a computer system that kept track of each robotics team's wins and losses. <br>

<br>
<u>SKILLS </u>
<br>Languages: 
<br>* Spanish - Proficient - Native/Bilingual <br>

    </p>
    <!-- Button that allows for users to download my resume as a file but It did not work as planed -->
    <a href="#" class="btn btn-warning mt-2 mb-3">Download My Resume</a>
  </div>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      // define my Skills, as a progress bar 
      skillProgress: [
        { title: "Html:", vNow: 85, vStyle: "80%" },
        { title: "Css:", vNow: 85, vStyle: "85%" },
        { title: "Bootstrap:", vNow: 60, vStyle: "60%" },
        { title: "Javascript:", vNow: 80, vStyle: "80%" },
        { title: "Vuejs:", vNow: 75, vStyle: "75%" },
        { title: "Vuejs:", vNow: 75, vStyle: "75%" },
        { title: "Axure", vNow: 75, vStyle: "75%" },
        { title: "Balsamiq Wireframes:", vNow: 80, vStyle: "80%" },
      ],
    };
  },
};
</script>

<style scoped>
h6 {
  margin: 1rem 0;
}
</style>
