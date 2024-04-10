<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
Ref: https://github.com/othneildrew/Best-README-Template/edit/master/README.md
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
<!-- 
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
-->


<!-- PROJECT LOGO -->
<!--
<br />
<p align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Best-README-Template</h3>

  <p align="center">
    An awesome README template to jumpstart your projects!
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a>
  </p>
</p>
-->


<!-- TABLE OF CONTENTS -->
<!--
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
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>
-->



<!-- ABOUT THE PROJECT -->
# Png Info to txt file for multiple png files generated by Stable Diffusion Webui

# About the project

While using Stable Diffusion Webui, I found it costs me a lot of time to copy, paste, and modified the png info into a single *.txt file. With this *.ipynb program, the png info in the png files are automatically gathered and formated into a single *.txt file for using in "Prompts from file or textbox" of txt2img in Stable Diffusion Webui.

In this very beginning version, `Positive prompt`, `Negative prompt`, `Width`, and `Height` are formatted and written to the "*.txt" file.

![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](code_of_conduct.md)


# Purpose
1. Extract the `Positive prompt value`, `Negative prompt value`, `width`, and `height` from the png files generated by Stable Diffusion Webui.
2. Format the `Positive prompt value`, `Negative prompt value`, `width`, and `height` for using in "Prompts from file or textbox" of Stable Diffusion Webui.
3. Output the formatted text in the `*.txt` file.
4. Batch process the above steps.

# Usage 1:
1. Put the `*.ipynb` file in the target folder (where you run the `*.ipynb` file).
2. Create a folder named `PNG files` under the target folder.
3. Put the target png files in the folder `PNG files`.
4. Run all cells in the `*.ipynb` file. Or use the hot key `Shift + Enter` to run the program, since just only one cell in the program.
5. A file named `png_info_collection.txt` will be created in the target folder after the process. It can be used in "Prompts from file or textbox" of Stable Diffusion Webui.

# Usage 2:
Modify the paths of the input and output folder by yourself. It's convenient for specific users.

# Suitable version of Stable Diffusion Webui
v1.7.0 (tested on Mar. 09 2024)

# About Stable Diffusion Webui

https://github.com/AUTOMATIC1111/stable-diffusion-webui

<!-- GETTING STARTED -->
<!--
# Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.
-->


<!-- USAGE EXAMPLES -->
# Version information

| #    | Source file                                                                                        | Date       |
| ---- | -------------------------------------------------------------------------------------------------- | ---------- |
|    4 | [PngInfo_To_Txt_ForMultiplePng_v04.ipynb](code/PngInfo_To_Txt_ForMultiplePng_v04.ipynb)            | 2024-04-08 |
|    3 | [PngInfo_To_Txt_ForMultiplePng_v03.ipynb](code/PngInfo_To_Txt_ForMultiplePng_v03.ipynb)            | 2024-03-09 |
|    2 | [PngInfo_To_Txt_ForMultiplePng_v02.ipynb](code/PngInfo_To_Txt_ForMultiplePng_v02.ipynb)            | 2024-02-06 |
|    1 | [PngInfo_To_Txt_ForMultiplePng_v01.ipynb](code/PngInfo_To_Txt_ForMultiplePng_v01.ipynb)            | 2024-02-06 |


# Limitation
Since the positive and negative prompts are enclosed by the symbol `"`, if you make a typo `"` in the positive and negative prompts, you will get wrong prompts and unexpected results.  
For example: If you type (masterpiece: 1.2) as (masterpiece" 1.2).

<!-- LICENSE -->
# License

Distributed under the [MIT License](LICENSE).



<!-- CONTACT -->
# Contact

Author: Dr. Hsien-Ching Chung

ORCiD: https://orcid.org/0000-0001-9364-8858

Project Link: [https://github.com/HsienChing/PngInfo_To_Txt_ForMultiplePng_StableDiffusionWebui](https://github.com/HsienChing/PngInfo_To_Txt_ForMultiplePng_StableDiffusionWebui)



<!-- ACKNOWLEDGEMENTS -->
<!--
# Acknowledgements

* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)
* [Animate.css](https://daneden.github.io/animate.css)
* [Loaders.css](https://connoratherton.com/loaders)
* [Slick Carousel](https://kenwheeler.github.io/slick)
* [Smooth Scroll](https://github.com/cferdinandi/smooth-scroll)
* [Sticky Kit](http://leafo.net/sticky-kit)
* [JVectorMap](http://jvectormap.com)
* [Font Awesome](https://fontawesome.com)

H.C. Chung thanks all the contributors to this project for their valuable discussions and recommendations, especially Jung-Feng Lin, Hsiao-Wen Yang, Yen-Kai Lo, An-De Andrew Chung.

This work was supported in part by Super Double Power Technology Co., Ltd., Taiwan under grant SDP-RD-PROJ-001-2020.
-->


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
<!--
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
-->
