---
#layout: default
title: LoRa Transceiver
permalink: /xcvr/
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

<body>
<!--
  <div class="row">
  <p> <b>LoRaWan Transceiver Board</b> </p>
  </div>
-->

  <div class="row">
  <section>
  <div class="indent2em">
  <p>
           The LoRa transceiver is designed to operate from 5.2VDC to 10VDC. A LDO regulator provides 5.0VDC to two 3.3VDC LDOs.
           <br>One 3.3V LDO regulator provides the digital power rails and the second 3.3V LDO provides power to the STM32 analog power input.
           <br>The 5.0VDC power rail is connected to J10 and the 3.3V power rail is connected to J8. 
   </p>
   </div>
   </section>
  </div>

  <div class="row">
  <section>
  <div>
  <p>
  <u>Revision 1</u>
  </p>
  </div>
  </section>
  </div>

  <div class="row">
  <div class="xcvrcolumn">
  <section>
  <ul> 
  <li>STM32L15xCCT6 : 
  <div class="indent2em">256K Flash Memory</div>
  <div class="indent2em">32K SRAM </div> 
  <div class="indent2em">RTC Support - 32Khz Crystal</div>
  </li>
  <br>
      
  <li>LoRa Transceiver Module 
  <div class="indent2em"> HopeRF RFM95W US 915Mhz FCC certified</div>
  </li>
  <br>
      
  <li> Debug Port
  <div class="indent2em"> RS-232 3.3V TTL </div> 
  </li>
  <br>

  <li>ST-LINK SWDIO Programming header
  </li>
  <br>

  <li>Input Voltage
  <div class="indent2em">5.2 to 10 volts DC (500mA max)</div>
  <div class="indent2em">Reverse polarity input protection (R2) </div>
  </li>
  <br>

  <li>Dimensions
  <div class="indent2em">2.5” x 3.5” (63.5 x76.2 mm)</div>
  </li>
  </ul>
  </section>

  </div>

  <img src="/assets/images/MainBoard_500x418.JPG"  style="width:auto;height:auto;">
  </div>
</body>


