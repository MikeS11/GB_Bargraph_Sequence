[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![Twitter][Twitter-shield]][Twitter-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/MikeS11/GB_Bargraph_Sequence">
    <img src="Images/MikeS11_Logo.jpg?raw=true" alt="Logo" width="180" height="200">
  </a>

  <h3 align="center">28 Segment Bargraph Library for Arduino Proton Packs</h3>

  <p align="center">
  This is for anyone who wants to add a more movie accurate bargraph to their Arduino projects.  

<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#Build-Requirements)
* [Getting Started](#getting-started)
  * [Circuit Pinouts](#circuit-pinouts)  
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)

<!-- ABOUT THE PROJECT -->
## About The Project

<p align="center">
<img src="Images/28SegBarGraph.png?raw=true" alt="Prototype" width="597" height="504"><img src="Images/HT16k33.png?raw=true" alt="Prototype" width="623" height="665"></p>
My original Spirit Halloween project was based on Eric Banker's (CountDeMonet's) 15 segment bargraph but I wanted something a bit more movie accurate. Seeing how there was no source online I decided to write my own library and share it to the GB community.

### Getting Started

### Build Requirements:

* []() 1 - 28 Segment Bargraph - Found on Ebay (Supplier BarMeter.com) 
* []() 1 - HT16K33 Breakout Board (Or Alternative)

Library Functions

    initiateVariables(uint8_t BGMODE);              - Initiate Variables based on mode
    changeInterval(uint8_t NewInterval);            - Change the bargraph speed 
    sequenceFire1(unsigned long currentMillis);     - Fire 1 Sequence
    sequenceFire2(unsigned long currentMillis);     - Fire 2 Sequence
    sequenceStart(unsigned long currentMillis);     - Wand Only on
    sequencePackOn(unsigned long currentMillis);    - Normal Pack on Sequence
    sequenceVent(unsigned long currentMillis);      - Vent Sequence
    clearLEDs();                                    - Clear all the LEDs
    sequenceShutdown(unsigned long currentMillis);  - Shutdown Sequence

### Circuit Pinouts:

Arduino to the HT16k33 Breakout Board  

    SCL ----- A5
    SDA ----- A4
    
Bargraph to the HT16k33 Breakout Board  

    5V 	    to 	VDD
    GND 	  to 	GND
    Pin 21	to 	C0
    Pin 15 	to 	C1
    Pin 13 	to 	C2
    Pin 16 	to 	C3
    Pin 22 	to	A0
    Pin 1 	to	A1
    Pin 19 	to	A2
    Pin 18 	to	A3
    Pin 7 	to	A4
    Pin 10 	to	A5
    Pin 7 	to	A6    
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<!-- CONTACT -->
## Contact

Mike Simone - [@mikesimone3](https://twitter.com/mikesimone3) 

Project Link: [https://github.com/MikeS11/GB_Bargraph_Sequence](https://github.com/MikeS11/ProtonPack)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/MikeS11/GB_Bargraph_Sequence.svg?style=flat-square
[contributors-url]: https://github.com/MikeS11/GB_Bargraph_Sequence/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/MikeS11/GB_Bargraph_Sequence.svg?style=flat-square
[forks-url]: https://github.com/MikeS11/GB_Bargraph_Sequence/network/members
[stars-shield]: https://img.shields.io/github/stars/MikeS11/GB_Bargraph_Sequence.svg?style=flat-square
[stars-url]: https://github.com/MikeS11/GB_Bargraph_Sequence/stargazers
[issues-shield]: https://img.shields.io/github/issues/MikeS11/GB_Bargraph_Sequence.svg?style=flat-square
[issues-url]: https://github.com/MikeS11/GB_Bargraph_Sequence/issues
[license-shield]: https://img.shields.io/github/license/MikeS11/GB_Bargraph_Sequence.svg?style=flat-square
[license-url]: https://github.com/MikeS11/GB_Bargraph_Sequence/blob/master/LICENSE.txt
[twitter-shield]: https://img.shields.io/badge/-Twitter-black.svg?style=flat-square&logo=Twitter&colorB=555
[twitter-url]: https://Twitter.com/mikesimone3
[product-screenshot]: images/screenshot.png

