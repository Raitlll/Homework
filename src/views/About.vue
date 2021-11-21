<template>
  <div class="about">
    <h1>Contact information</h1>
  </div>
  <div class="row">
    <div class="column">
      <div class="person">
        <p class="job">CEO</p>
        <p>Mart Saar</p>
        <p>martsaar@postit.com</p>
        <p>+37256728525</p>
      </div>
      <div class="person">
        <p class="job">Project Manager</p>
        <p>Mari Tamm</p>
        <p>maritamm@postit.com</p>
        <p>+372512452356</p>
      </div>
      <div class="person">
        <p class="job">Recruitment Manager</p>
        <p>Peeter Paan</p>
        <p>peeterpaan@postit.com</p>
        <p>+372545222356</p>
      </div>
    </div>
    <div class="column">
      <div class="person">
        <p class="job">PR Manager</p>
        <p>Marju Kass</p>
        <p>marjukass@postit.com</p>
        <p>+37254256246</p>
      </div>
      <div class="person">
        <p class="job">Head Analyst</p>
        <p>Marko Tamm</p>
        <p>markotamm@postit.com</p>
        <p>+37255235236</p>
      </div>
      <div class="person">
        <p class="job">Tester</p>
        <p>Alexandra Kallustik</p>
        <p>alexandra.kallustik@postit.com</p>
        <p>+37252665756</p>
      </div>
    </div>
  <div class="office">
    <p>Street 12, Tallinn, Estonia</p>
  </div>
  </div>
</template>

<style>
 .column{
   float: left;
   width: 50%;
 }
 .row{
   background-color: #f49f1c;
 }
 .row:after{
   content: "";
   display: table;
   clear:both;
 }
 .person{
   border-style: solid;
   border-color: whitesmoke;
   margin: 10px;
 }
 .office{
   font-weight: bolder;
 }
 .job {
   font-weight: bold;
 }
 .about{
   color: #f49f1c;
 }
 p{
   color: black;
 }
</style>