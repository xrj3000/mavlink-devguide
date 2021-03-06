<!-- THIS FILE IS AUTO-GENERATED: https://github.com/mavlink/mavlink/blob/master/doc/mavlink_gitbook.py -->

# MAVLINK Message Set: ualberta.xml

*This is a human-readable form of the XML definition file: [ualberta.xml](https://github.com/mavlink/mavlink/blob/master/message_definitions/v1.0/ualberta.xml).*

<span></span>

> **Note** MAVLink 2 messages have an ID > 255 and are marked up using **(MAVLink 2)** in their description.

<span id="mav2_extension_field"></span>

> **Note** MAVLink 2 extension fields that have been added to MAVLink 1 messages are displayed in blue. 

<style>
td {
    vertical-align:top;
}
</style>

 <html>
 <body></p>

<p>
   <strong>MAVLink Include Files:</strong>
   <a href="common.md">common.xml</a>
  </p>

<h2>MAVLink Type Enumerations</h2>

<h3 id="UALBERTA_AUTOPILOT_MODE">
   <a href="#UALBERTA_AUTOPILOT_MODE">UALBERTA_AUTOPILOT_MODE</a>
  </h3>

<p>Available autopilot modes for ualberta uav</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="MODE_MANUAL_DIRECT">
     <td>
     </td>
     <td>
      <a href="#MODE_MANUAL_DIRECT">MODE_MANUAL_DIRECT</a>
     </td>
     <td>Raw input pulse widts sent to output</td>
    </tr>
    <tr id="MODE_MANUAL_SCALED">
     <td>
     </td>
     <td>
      <a href="#MODE_MANUAL_SCALED">MODE_MANUAL_SCALED</a>
     </td>
     <td>Inputs are normalized using calibration, the converted back to raw pulse widths for output</td>
    </tr>
    <tr id="MODE_AUTO_PID_ATT">
     <td>
     </td>
     <td>
      <a href="#MODE_AUTO_PID_ATT">MODE_AUTO_PID_ATT</a>
     </td>
     <td>dfsdfs</td>
    </tr>
    <tr id="MODE_AUTO_PID_VEL">
     <td>
     </td>
     <td>
      <a href="#MODE_AUTO_PID_VEL">MODE_AUTO_PID_VEL</a>
     </td>
     <td>dfsfds</td>
    </tr>
    <tr id="MODE_AUTO_PID_POS">
     <td>
     </td>
     <td>
      <a href="#MODE_AUTO_PID_POS">MODE_AUTO_PID_POS</a>
     </td>
     <td>dfsdfsdfs</td>
    </tr>
   </tbody>
  </table>

<h3 id="UALBERTA_NAV_MODE">
   <a href="#UALBERTA_NAV_MODE">UALBERTA_NAV_MODE</a>
  </h3>

<p>Navigation filter mode</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="NAV_AHRS_INIT">
     <td>
     </td>
     <td>
      <a href="#NAV_AHRS_INIT">NAV_AHRS_INIT</a>
     </td>
     <td>
     </td>
    </tr>
    <tr id="NAV_AHRS">
     <td>
     </td>
     <td>
      <a href="#NAV_AHRS">NAV_AHRS</a>
     </td>
     <td>AHRS mode</td>
    </tr>
    <tr id="NAV_INS_GPS_INIT">
     <td>
     </td>
     <td>
      <a href="#NAV_INS_GPS_INIT">NAV_INS_GPS_INIT</a>
     </td>
     <td>INS/GPS initialization mode</td>
    </tr>
    <tr id="NAV_INS_GPS">
     <td>
     </td>
     <td>
      <a href="#NAV_INS_GPS">NAV_INS_GPS</a>
     </td>
     <td>INS/GPS mode</td>
    </tr>
   </tbody>
  </table>

<h3 id="UALBERTA_PILOT_MODE">
   <a href="#UALBERTA_PILOT_MODE">UALBERTA_PILOT_MODE</a>
  </h3>

<p>Mode currently commanded by pilot</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="PILOT_MANUAL">
     <td>
     </td>
     <td>
      <a href="#PILOT_MANUAL">PILOT_MANUAL</a>
     </td>
     <td>sdf</td>
    </tr>
    <tr id="PILOT_AUTO">
     <td>
     </td>
     <td>
      <a href="#PILOT_AUTO">PILOT_AUTO</a>
     </td>
     <td>dfs</td>
    </tr>
    <tr id="PILOT_ROTO">
     <td>
     </td>
     <td>
      <a href="#PILOT_ROTO">PILOT_ROTO</a>
     </td>
     <td>Rotomotion mode</td>
    </tr>
   </tbody>
  </table>

<h2>MAVLink Messages</h2>

<h3 id="NAV_FILTER_BIAS">NAV_FILTER_BIAS (<a href="#NAV_FILTER_BIAS">
    #220
   </a>
   )
  </h3>

<p>Accelerometer and Gyro biases from the navigation filter</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Field Name</th>
     <th>Type</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr>
     <td>usec</td>
     <td>uint64_t</td>
     <td>Timestamp (microseconds)</td>
    </tr>
    <tr>
     <td>accel_0</td>
     <td>float</td>
     <td>b_f[0]</td>
    </tr>
    <tr>
     <td>accel_1</td>
     <td>float</td>
     <td>b_f[1]</td>
    </tr>
    <tr>
     <td>accel_2</td>
     <td>float</td>
     <td>b_f[2]</td>
    </tr>
    <tr>
     <td>gyro_0</td>
     <td>float</td>
     <td>b_f[0]</td>
    </tr>
    <tr>
     <td>gyro_1</td>
     <td>float</td>
     <td>b_f[1]</td>
    </tr>
    <tr>
     <td>gyro_2</td>
     <td>float</td>
     <td>b_f[2]</td>
    </tr>
   </tbody>
  </table>

<h3 id="RADIO_CALIBRATION">RADIO_CALIBRATION (<a href="#RADIO_CALIBRATION">
    #221
   </a>
   )
  </h3>

<p>Complete set of calibration parameters for the radio</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Field Name</th>
     <th>Type</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr>
     <td>aileron</td>
     <td>uint16_t[3]</td>
     <td>Aileron setpoints: left, center, right</td>
    </tr>
    <tr>
     <td>elevator</td>
     <td>uint16_t[3]</td>
     <td>Elevator setpoints: nose down, center, nose up</td>
    </tr>
    <tr>
     <td>rudder</td>
     <td>uint16_t[3]</td>
     <td>Rudder setpoints: nose left, center, nose right</td>
    </tr>
    <tr>
     <td>gyro</td>
     <td>uint16_t[2]</td>
     <td>Tail gyro mode/gain setpoints: heading hold, rate mode</td>
    </tr>
    <tr>
     <td>pitch</td>
     <td>uint16_t[5]</td>
     <td>Pitch curve setpoints (every 25%)</td>
    </tr>
    <tr>
     <td>throttle</td>
     <td>uint16_t[5]</td>
     <td>Throttle curve setpoints (every 25%)</td>
    </tr>
   </tbody>
  </table>

<h3 id="UALBERTA_SYS_STATUS">UALBERTA_SYS_STATUS (<a href="#UALBERTA_SYS_STATUS">
    #222
   </a>
   )
  </h3>

<p>System status specific to ualberta uav</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Field Name</th>
     <th>Type</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr>
     <td>mode</td>
     <td>uint8_t</td>
     <td>System mode, see UALBERTA_AUTOPILOT_MODE ENUM</td>
    </tr>
    <tr>
     <td>nav_mode</td>
     <td>uint8_t</td>
     <td>Navigation mode, see UALBERTA_NAV_MODE ENUM</td>
    </tr>
    <tr>
     <td>pilot</td>
     <td>uint8_t</td>
     <td>Pilot mode, see UALBERTA_PILOT_MODE</td>
    </tr>
   </tbody>
  </table>

<p></body>
</html>
