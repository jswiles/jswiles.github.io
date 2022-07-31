---
layout: default
title: Solar Charger
permalink: /solcon/
---

<style>
.xcvrcolumn {
  float: left ;
  width: 30.00%;
  padding: 15px;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

</style>

  <p> <b> Solar Charge Controller </b> </p>

  <div class="row">
      <section>
          <a style="color:blue;" href="/solcon" {% if page.title == "Solar Charger" %}class="active-page"{% endif %}>MPPTSolarPwrModule_R2</a>
      </section>
  </div>



  <div class="row">
      <section>
         <div class="indent2em">
         <p>
           The solar charge controller board uses LT3652HV MPPT power tracking battery charger IC. Revision 1 is set to charge a 7.4 LiPO battery pack with a 3 pin JST connector. 
         </p>
         </div>
      </section>
  </div>


  <div class="row">
      <section>
         <div>
         <p>
           <u>Solar Charge Controller Revision 1</u>
         </p>
         </div>
      </section>
  </div>


  <div class="row">

    <div class="xcvrcolumn">
      <section>
         <ul>
         <li>
             Solar Panel Support:
             <br> 12V Solar Panel Input – 17.5V open circuit, 12.5V nominal
         </li>
         <br>

         <li>
            Battery:
            <br> 7.4V 2S LiPO (default configuration)
         </li>
         <br>

         <li>
             Dimensions:   
         </li>
         </ul>
      </section>

    </div>
    <img src="/assets/images/SolarCharger_500x236.JPG"  style="width:auto;height:auto;">
  </div>

