<h1>📡 BLE Beacon Information System</h1>

<div style="border: 1px solid black; padding: 10px;">

<p>
  This project was developed as part of the <strong>Mobility in Computational Systems</strong> course in the Computer Engineering (Mobile Computing) Master's degree during the 2023/24 academic year.
</p>

<h1>Collaborators</h1>
<ul>
  <li><a href="https://github.com/anamsmartins">Ana Martins</a></li>
</ul>

<h1>Project Description</h1>

<p>
<strong>Exploring Bluetooth Low Energy (BLE) Beaconing for Showing Information</strong> is a mobile-based
project focused on using BLE beacons to display contextual information to users based on proximity.
The system was designed with museum environments in mind, where users can receive supplementary
information about artworks when they are nearby.
</p>

<p>
The project explores a feasible approach to scanning BLE beacon signals, analysing their RSSI values,
and redirecting users to the most relevant information source according to the strongest detected beacon.
</p>

<p>
Two BLE Ruuvi beacons and an Android smartphone were used to test signal behaviour, advertising intervals,
maximum indoor and outdoor range, and RSSI-based accuracy.
</p>

<h1>System Architecture</h1>

<p>
The system is composed of BLE beacons positioned near points of interest, users carrying mobile devices,
and an Android application responsible for scanning, processing, and displaying information.
</p>

<ul>
  <li>BLE Beacons broadcasting advertising signals</li>
  <li>Android smartphone running the scanning application</li>
  <li>Information pages associated with each beacon</li>
</ul>

<h1>Main Features</h1>

<ul>
  <li>Active scanning of BLE advertising signals</li>
  <li>MAC address identification for known beacons</li>
  <li>RSSI-based comparison to determine closest beacon</li>
  <li>Automatic redirection to beacon-specific information</li>
  <li>Information update intervals of 30 seconds</li>
</ul>

<h1>Tested Devices</h1>

<h2>BLE Beacons</h2>
<ul>
  <li><strong>Ruuvi Beacon 1</strong>
    <ul>
      <li>Bluetooth version: 4.1</li>
      <li>Hardware version: B7.1</li>
      <li>Battery: CR2477 3V</li>
    </ul>
  </li>
  <li><strong>Ruuvi Beacon 2</strong>
    <ul>
      <li>Bluetooth version: 4.1</li>
      <li>Hardware version: B6</li>
      <li>Battery: CR2477 3V</li>
    </ul>
  </li>
</ul>

<h2>Mobile Device</h2>
<ul>
  <li>Android smartphone (Android 13)</li>
  <li>Bluetooth version 5.0</li>
</ul>

<h1>Evaluation & Tests</h1>

<h2>Advertising Interval Tests</h2>
<p>
Multiple scans were conducted to analyse beacon boot time, first signal detection, and advertising intervals.
Results showed inconsistent advertising intervals and differences between the two beacons, especially after
extended periods of operation.
</p>

<h2>Maximum Distance Tests</h2>
<ul>
  <li><strong>Outdoor Range:</strong>
    <ul>
      <li>Beacon 1: ~131.5 meters</li>
      <li>Beacon 2: ~79.2 meters</li>
    </ul>
  </li>
  <li><strong>Indoor Range:</strong>
    <ul>
      <li>Beacon 1: ~16.5 meters</li>
      <li>Beacon 2: ~17.1 meters</li>
    </ul>
  </li>
</ul>

<h2>Accuracy Based on RSSI</h2>
<p>
Accuracy tests based solely on RSSI values showed reliable detection when users were very close to a beacon.
However, when positioned between multiple beacons, signal fluctuations led to inconsistent results.
</p>

<h1>Results & Discussion</h1>

<p>
The system demonstrated high accuracy in close-proximity scenarios but struggled in environments where
multiple beacon signals overlapped. RSSI values showed non-linear and random fluctuations, making it
difficult to implement a reliable linear correction method.
</p>

<p>
It was also observed that beacon detection efficiency decreased after prolonged operation, requiring
manual resets to restore performance — a limitation for real-world deployments such as museums.
</p>

<h1>Conclusion</h1>

<p>
This project successfully demonstrates a feasible process for using BLE beacons to display contextual
information based on proximity. While RSSI-based methods alone are insufficient for high-accuracy
localization, the study provides valuable insights into beacon behaviour, limitations, and performance
characteristics.
</p>

<h1>Future Work</h1>
<ul>
  <li>Implementation of distance-based localization methods</li>
  <li>Fingerprint-based approaches using RSSI maps</li>
  <li>Testing with dynamic noise and crowded environments</li>
  <li>Improved accuracy through machine learning techniques</li>
</ul>

<h1>Tools & Technologies</h1>
<ul>
  <li>Android Studio – Mobile development</li>
  <li>Java / Android SDK</li>
  <li>BLE Ruuvi Beacons</li>
  <li>Bluetooth Low Energy (BLE)</li>
</ul>


<h1>Other Information</h1>
<ul>
  <li><strong>The project received a grade of 15.20 out of 20.</strong></li>
  <li>This project was developed for the <a href="https://www.ipleiria.pt/curso/mestrado-em-engenharia-informatica-computacao-movel/" rel="nofollow">Computer Engineering (Mobile Computing) master's degree</a> at <a href="https://www.ipleiria.pt" rel="nofollow">Polytechnic of Leiria</a></li>
</ul>

<p>
<a href="https://www.ipleiria.pt/estg/" rel="nofollow">
<img src="https://www.ipleiria.pt/normasgraficas/wp-content/uploads/sites/80/2017/09/estg_h-01.jpg"
     width="300"
     alt="Escola Superior de Tecnologia e Gestão"
     style="max-width: 100%;">
</a>
</p>

</div>
