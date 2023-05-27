<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/camiloms10/f1dashboard">
    <img src="images/logo-F1.png" alt="Logo" width="150" height="80">
  </a>

<h3 align="center">F1 Power BI Dashboard</h3>

  <p align="center">
    This project was made using Power BI, to generate a working dataset and report based of F1 data such as: laptimes, results, races, qualifyings, etc.
    <br />
    <a href="https://github.com/camiloms10/f1dashboard"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/camiloms10/f1dashboard/issues">Report Bug</a>
    ·
    <a href="https://github.com/camiloms10/f1dashboard/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <!--li><a href="#prerequisites">Prerequisites</a></li-->
        <li><a href="#data-sources">Data Sources</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <!--<li><a href="#contributing">Contributing</a></li>-->
    <!--<li><a href="#license">License</a></li>-->
    <li><a href="#contact">Contact</a></li>
    <!--<li><a href="#acknowledgments">Acknowledgments</a></li>-->
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<img src="images/logo-F1.png" alt="Logo" width="150" height="80">

Through this project you´ll find an interactive report in which you can find different views to analyze and visualize F1 data and metrics from different perspectives such as: by driver (nationality and name), by season, by constructor (nationality and name), by circuit (country and specific circuit), etc.
<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [Power BI](https://powerbi.microsoft.com/es-es/desktop/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started


<!--### Prerequisites

These are the python libraries you´ll need to run the ipynb file.
* Libraries
  ```sh
  pip install numpy
  pip install seaborn 
  pip install matplotlib
  pip install pandas
  pip install sklearn 
  pip install scipy
   ```
-->

<p align="right">(<a href="#top">back to top</a>)</p>

### Data Sources

Formula 1 race data from the years 1950 to 2017. This data set is based on Formula 1 Race Data by ChrisG. As ChrisG indicated, the data was downloaded from http://ergast.com/mrd/ at the conclusion of the 2017 season.

I downloaded the data source of this project from [Kaggle](https://www.kaggle.com/datasets/davidcochran/formula-1-race-data-sqlite), it's a SQLite database called Formula1.sqlite.

  * Formula1.sqlite contains these 13 tables:
    * circuits
    * constructor_standings
    * constructor_results
    * constructors
    * driver_standings
    * drivers
    * laptimes
    * pitstops
    * qualifying
    * races
    * results
    * seasons
    * status


<p align="right">(<a href="#top">back to top</a>)</p>




<!-- USAGE EXAMPLES -->
## Usage

You can use this data to analyze:
* How a driver or constructor has performed through time
* Compare drivers and/or constructors based on F1 key metrics
* Easily obtain the top performers for a specific F1 key metric
* Ranking the constructor and drivers based on their performance 
* Etc.
<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

To do ALL of the following report and dataset I used Power BI Desktop.

### 1. Importing the data into Power BI Desktop

<p align ="center">

![grab-landing-page](https://github.com/camiloms10/f1dashboard/blob/master/images/PBI-import-_1_.gif?raw=true)


* I've used the ODBC connection to import the SQLite database into Power BI, selecting each one of the tables and making sure the data types of the columns correspond to what they're meant to be (decimal number, whole number, text, etc.).


### 2. Managing the model relationships

<p align ="center">

![grab-landing-page](https://raw.githubusercontent.com/camiloms10/f1dashboard/master/images/Relationships.gif)

<p align ="center">
Now I've set the relationships between the tables in order to follow a star model (as it should be in Power BI), where we find the fact table(s) in the center of the model and the dimension or catalog tables surrounding the fact table.
</p>

<p align ="left">
The fact and dimension tables have been classified as follows...

* Fact tables:
  * Results
  * Qualifyings
  * Races
  * Laptimes
  * Pitstops
* Dimension tables:
  * Drivers
  * Constructors
  * Circuits
  * Seasons
</p>
</p>


### 3. Using all of 2021-2020 quantitative statistics

<p align ="center">

</p>
<p align ="center">
<img src="images/quantitative_stats_model_error.png" width="400" height="300">
<p align ="center">

</p>
</p>



### 4. Variables significance (p-value <.05)

<p align ="center">

</p>

<p align ="center">
<img src="images/significant_variables_error_distributions.png" width="400" height="300">
<p align ="center">

</p>
</p>


## Final Conclusions



See the [open issues](https://github.com/camiloms10/f1dashboard/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING 
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>
-->


<!-- LICENSE 
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>
-->


<!-- CONTACT -->
## Contact

Camilo Manzur - [@LinkedIn](https://www.linkedin.com/in/camilo-manzur-4b7137a8/)

Project Link: [https://github.com/camiloms10/f1dashboard/](https://github.com/camiloms10/f1dashboard)


Portfolio Link: [https://camiloms10.github.io/](https://camiloms10.github.io/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS 
## Acknowledgments

* []()
* []()
* []()

<p align="right">(<a href="#top">back to top</a>)</p>
-->


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/camiloms10/soccer_players_value.svg?style=for-the-badge
[contributors-url]: https://github.com/camiloms10/f1dashboard/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/camiloms10/soccer_players_value.svg?style=for-the-badge
[forks-url]: https://github.com/camiloms10/f1dashboard/network/members
[stars-shield]: https://img.shields.io/github/stars/camiloms10/soccer_players_value.svg?style=for-the-badge
[stars-url]: https://github.com/camiloms10/f1dashboard/stargazers
[issues-shield]: https://img.shields.io/github/issues/camiloms10/soccer_players_value.svg?style=for-the-badge
[issues-url]: https://github.com/camiloms10/f1dashboard/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/camilo-manzur-4b7137a8/
[product-screenshot]: images/screenshot.png