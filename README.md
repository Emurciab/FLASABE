<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/Emurciab/FLASABE.git">
    <img src="Test Forecast S7 EEMD.png" alt="Logo" width="150" height="150">
  </a>

  <h3 align="center">README</h3>

  <p align="center">
    Hybrid ML: Implementation of a Mixture of Experts (MoE) ensemble algorithm in a soil moisture forecasting task.!
    <br />
    <a href="https://github.com/Emurciab/FLASABE.git"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#usage">View Demo</a>
    ·
    <a href="https://github.com/Emurciab/FLASABE.git">Report Bug</a>
    ·
    <a href="https://github.com/Emurciab/FLASABE.git">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
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
        <li><a href="#dependencies">Dependencies</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#authors">Authors</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

_For a video with explaining the scope of the  project and more in detail information please visit [here](https://youtu.be/WE8JMwTLO60)_


Accurate estimations of soil water content are needed to create decision-support systems for irrigation management in agriculture. Hybrid approaches combining signal preprocessing techniques and ensemble learning algorithms could provide the necessary accuracy for a reliable machine learning (ML) forecast system.

In our lab we had first-hand experience working with soil moisture sensors data for irrigation management and from there we identified the following challenges:
 
- Complexity created from non-linear and non-stationary time series.
- Single algorithms are limited to performing well only on specific parts of the data. 

To tackle the complexity we implemented a hybrid apptoach that combines signal preprocesssing techniques with ML. Thus, two ML algorithms, namely LSTM-ED and RF, and two signal preprocessing techniques, namely SSA and EEMD, were integrated and evaluated to determine whether decomposing the original TS would ease the learning task for the algorithm.

To overcome the limitations of single algorithms, we have implemented a Mixture of Experts (MoE) approach that use a Gaussian Gating Network to determine the contribution that each 'expert'model on the point estimation.

Note: This is project is currently being developed. Once completed we will provide access to the code files and data that we have used and generated.

[Hybrid ML: Implementation of a Mixture of Experts (MoE) ensemble algorithm in a soil moisture forecasting task.!](https://github.com/Emurciab/FLASABE.git)



<!-- GETTING STARTED -->
## Getting Started

### Dependencies

This dependencies will be required for the code file that we will upload as soon as the project is completed.

* optuna: 3.1.1
  ```sh
  pip install optuna
  ```

### Alternative: Export your Environment

The yml file with the required dependencies is [here](https://github.com/uf-eel6825-sp23/final-project-code-Emurciab/requirements.yml)

  ```sh
  conda env export > requirements.yml
  ```

The user will be able to recreate it using:

  ```sh
  conda env create -f requirements.yml
  ```

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/uf-eel6825-sp23/final-project-code-Emurciab
   ```
2. Setup (and activate) your environment
  ```sh
  conda env create -f requirements.yml
  ```

<!-- USAGE EXAMPLES -->
## Usage

This project can be useful for anyone iterested in buliding ensemble ML algorithms for any forecasting tasks. In this case it is applied to an especific case of soil moisture but this carchitecture works as well for any task if the appropried formating and data QA/QC is performed.


_For a video with explaining the scope of the  project and more in detail information please visit [here](https://youtu.be/WE8JMwTLO60)_



<!-- Authors -->
## Authors

Eduart Murcia - [@EduartMurcia](https://twitter.com/EduartMurcia) - emurciabotache@ufl.edu

Project Link: [https://github.com/Emurciab/FLASABE.git](https://github.com/Emurciab/FLASABE.git)


<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

You can acknowledge any individual, group, institution or service.
* [Catia Silva](https://faculty.eng.ufl.edu/catia-silva/)

