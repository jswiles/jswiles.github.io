---
layout: default
title: Integrate
permalink: /integrate/
---

  <h1 style="text-align:center"> The Things Network Integrations  </h1>

  <p> The following are example integrations for The Things Newtork (V3) to 
  Ubidots or Thingspeak.
  </p>

  <h4> TTN Ubidots Webhook </h4>

  <p> Webhook base URL: <br> https://dataplugin.ubidots.com </p>

  <p>
     <h4> TTN Ubidots Uplink Decode Example </h4>
  </p>

  <pre><code>
function decodeUplink(input) {
  var data = {};

  data.battV = (input.bytes[0] << 8) | input.bytes[1];
  data.tC_probe = (input.bytes[2] << 8) | input.bytes[3];
  data.tC_si702x = (input.bytes[4] << 8) | input.bytes[5];
  data.Humidity_si702x = (input.bytes[6] << 8) | input.bytes[7];
  data.UVlevel = (input.bytes[8] << 16) | (input.bytes[9] << 8) | input.bytes[10];
  return {
    data: data
  };
}
  </code></pre>
  
  <p>
     <h2> Ubidots IoT Application </h2>
  </p>

  <h4> Ubidots Decoder Example </h4> 

  <pre><code>
function decodeUplink(bytes) {
  
  var decoded = {};
  var raw_humidity ;
  var calc_humidity ;
  var humidity_offset_lt80 ;
  var humidity_offset_gt80 ;
  

  //if (bytes[0] == 1) {
      // If received data is of Environment Monitoring type
      decoded.battV = ((bytes[0] << 8 | (bytes[1])) / 1000) * 4;

      decoded.tC_probe = ((bytes[2]<<24>>16 | (bytes[3])) / 100) * 9/5 +32;
      decoded.tC_si702x = ((bytes[4]<<24>>16 | (bytes[5])) / 10) * 9/5 + 32;

      raw_humidity = ((bytes[6] << 8 | bytes[7])) ;
      
      if (raw_humidity >= 1000) {
        raw_humidity = 1000 ;
      }
      calc_humidity = raw_humidity/10 ;

      decoded.humidity_si702x = calc_humidity;
      
      decoded.UVlevel = (bytes[8] << 16) | (bytes[9] << 8) | bytes[10] ;
  
  //} 
  return {"data": decoded};
}
  </code></pre>

  <p>
     <h3> Ubidots Dashboard </h3>
  </p>
  <figure>
    <img src="/assets/images/ubidots_22_03_16_scale.png"  style="width:auto;height:auto;">
  </figure>

  <p>
     <h2> ThingSpeak IoT Analytics </h2>
  </p>


  <h4> Thingspeak </h4>

  <p> Webhook base URL: <br>https://api.thingspeak.com/things_network/v3/update </p>

  <p>
     <h4> Thingspeak IoT Analytics Uplink Decode Example  </h4>
  </p>

  <pre><code>
function Decoder(b, port) {
  var var1 = (((b[0] << 8) | b[1]) / 1000) * 4 ;
  var var2 = (((b[2]<<24>>16)| b[3])/100) ;
  var var3 = (b[4] << 8) | b[5];
  var var4 = (b[6] << 8) | b[7];
  var var5 = (b[8] << 16) | (b[9] << 8) | b[10];
  var var6 = 0 ;
  var var7 = 0 ;
  var var8 = 0 ;

  return {
    field1: var1,
    field2: var2,
    field3: var3,
    field4: var4,
    field5: var5,
    field6: var6,
    field7: var7,
    field8: var8
  }
}
  </code></pre>


