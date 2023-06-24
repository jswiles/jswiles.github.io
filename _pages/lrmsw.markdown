---
layout: default
#title: LRMS
permalink: /lrms/
---

<style>
.xcvrcolumn {
  float: left;
  width: 30.00%;
  padding: 15px;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

</style>

  <div class="row">
  <section>
  <nav>
  <b>LoRaWan Remote Monitoring System (LRMS) </b>
  <ul>
  <li> <a style="color:blue;" href="/xcvr" {% if page.title == "LoRa Xcvr" %}class="active-page"{% endif %}>LoRa Transceiver Node</a></li>
  <li> <a style="color:blue;" href="/sensio" {% if page.title == "Sensor I/O" %}class="active-page"{% endif %}>Interface Boards</a></li>
  <li> <a style="color:blue;" href="/solcon" {% if page.title == "Solar Charger" %}class="active-page"{% endif %}>Solar Power Module</a> </li>
  <li> <a style="color:blue;" href="/sensors" {% if page.title == "Sensor" %}class="active-page"{% endif %}>Sensors</a> </li>
  <li> <a style="color:blue;" href="/enclosure" {% if page.title == "Monitor Enclosure" %}class="active-page"{% endif %}>Monitor System</a> </li>
  <li> <a style="color:blue;" href="/software" {% if page.title == "Software" %}class="active-page"{% endif %}>Software</a></li>
  <li> <a style="color:blue;" href="/integrate" {% if page.title == "Integrate" %}class="active-page"{% endif %}> TTN/Thingspeak Integration</a></li>
  </ul>
  </nav>
  </section>
  </div>

  <div class="row">
  <p>  </p> 
  </div>

  <div class="row">

  <div class="xcvrcolumn">
  <section>
  <div class="indent2em">
  <p>
  The LRMS project started in February of 2021 with the goal to create a flexible LoRaWan system design to support interfacing
  to multiple sensor types. 

  The prototype was based on available off the shelf development boards, component modules, and prototyping boards.   

  A Nucleo STM32 development board was chosen for I/O flexibilty, the capability to connect to Arduino prototyping boards, 
  stack variety of sensor modules, and develop software using the Arduino software development platform.

  As the prototype developed the scope changed to designing a complete system that could be connected
  to LoRaWan gateway and application server. 

  </p>
  </div>
  </section>

  <div class="row">
  <section>
  <div>
  <p><u>The Prototype</u></p>
  </div>
  </section>
  </div>

  <section>
  <div>
  <div><b>STM32 Development Board</b></div>
  <div class="indent2em">Nucleo-64 STM32L452</div>
  <br>
  </div>
  </section>
  <section>
  <div>
  <div><b>Sensors/Modules</b></div>
  <div class="indent2em"><b>Top board</b></div>
  <div class="indent2em"> MLP3115A2 Barometric/Altitude/Temperature Sensor</div>
  <div class="indent2em"> Si7021 Humidity/Temperature Sensor</div>
  <div class="indent2em"> LTR390 ALS/UV Sensor</div>
  <div class="indent2em"> Honeywell HPM Particulate Sensor</div>
  <div class="indent2em"> 24LC32 EEProm</div>
  <br>
  <div class="indent2em"><b>Middle board</b></div>
  <div class="indent2em"> UBLOX NEO-6M GPS Module</div>
  <div class="indent2em"> Adafruit RFM95 LoRa Transceiver</div>
  </div>
  </section>

  </div>
  <img src="/assets/images/ProtoType_Sensors_500x477.JPG"  style="width:auto;height:auto;">
  <img src="/assets/images/ProtoType_GPS_500x332.JPG"  style="width:auto;height:auto;">
</div>

<div class="indent2em">
   <p>
   Software is developed with the Arduino IDE, libraries, and STM32 board support package to create a modular design, with a focus on ease of implementation.
   <ul>
   <li>Arduino IDE based using Arduino CLI </li>
   <li>Arduino board support packages </li>
   <li>Arduino LMIC library </li>
   <li>Arduino libraries for devices </li>
   <li>STM32Lxxx Board Support Packages </li>
   </ul>
   </p>
</div>


<div class="indent2em">
   <p>
   Schematic, Board and mounting hardware are designed with the following CAD tools.
   <ul>
   <li>KiCad for schematic and board layout/design </li>
   <li>FreeCad for the design of 3D printed mounting plates, sensor supports, etc </li>
   </ul>
   </p>
</div>

