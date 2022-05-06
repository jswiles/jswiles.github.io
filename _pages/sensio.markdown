---
layout: default
title: Sensor I/O
permalink: /sensio/
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

  <p> <b> Interface Boards </b> </p>

  <div class="row">
      <section>
         <div>
         <p>
           <u>Sensor Terminal I/O Board Revision 1</u>
         </p>
         </div>
      </section>
  </div>

  <div class="row">
      <section>
         <div class="indent2em">
         <p>
           The sensor I/O terminal board has (3) 1x12 screw terminal blocks to connect to sensor modules via I2C, UART, SPI, ADC/DAC, GPIO input and outputs.
           <br>A I2C bus accelerator supports long cable lengths on the I2C bus.  
           The EEPROM provides static storage for LoRaWan EUI, board ID/type etc. 
         </p>
         </div>
      </section>
  </div>


  <div class="row">

    <div class="xcvrcolumn">
      <section>
         <ul>
         <li>
             EEPROM
             <div class="indent2em"> 24LC32A 4K byte</div> 
         </li>
         <br>

         <li>
            Serial I/O
            <div class="indent2em">UART1 – Debug port  </div>
            <div class="indent2em">UART2 – User port </div> 
         </li>
         <br>

         <li>
             I2C Busses 
             <div class="indent2em"> I2C1 -  On Board EEPROM </div> 
             <div class="indent2em"> I2C2 (J1) - LTC4311 I2C Bus Accelerator</div> 
         </li>
         <br>

         <li>
              3x -12 Position Screw Terminals (2.54mm) 
             <div class="indent2em"> J1 - I2C </div> 
             <div class="indent2em"> J2 - ADC,DAC, UART2 </div> 
             <div class="indent2em"> J3 - GPIO </div> 
         </li>
         <br>

         <li>
             Dimensions
             <div class="indent2em"> 2.5” x 3.0” </div> 
         </li>
         </ul>
      </section>
    </div>

    <img src="/assets/images/SenTermIOBrd_500x413.JPG"  style="width:auto;height:auto;">
  </div>

