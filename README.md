<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
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

![Salesforce](https://img.shields.io/badge/Salesforce-00A1E0?style=for-the-badge&logo=Salesforce&logoColor=white)
![VSCode](https://img.shields.io/badge/Visual_Studio-0078d7?style=for-the-badge&logo=visual%20studio&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="https://static.wikia.nocookie.net/logopedia/images/b/b1/Trailhead_old.svg/revision/latest?cb=20210528175818" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Trailhead Dev</h3>

  <p align="center">
    A collection of metadata changes from specific trailhead modules
    <a href="hhttps://github.com/MkHunter/trailhead-dev/wiki"><strong>Explore the docs »</strong></a>
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installing-the-app-using-a-scratch-org">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

This repo holds metadata changes as a result of completing several trailhead badges.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
Set up your environment. Follow the steps in the [Quick Start: Lightning Web Components](https://trailhead.salesforce.com/content/learn/projects/quick-start-lightning-web-components/) Trailhead badge. The steps include:

  - Enable Dev Hub in your Trailhead Playground
  - Install [Salesforce CLI](https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_install_cli.htm)
  - Install [Visual Studio Code](https://code.visualstudio.com/download)
  - Install the [Visual Studio Code Salesforce extensions](https://marketplace.visualstudio.com/items?itemName=salesforce.salesforcedx-vscode)
  - Install [ApexDox VS Code](https://marketplace.visualstudio.com/items?itemName=PeterWeinberg.apexdox-vs-code#special-tokens)

### Installing the app using a Scratch Org

1. If you haven't already done so, authorize your hub org and provide it with an alias (**myhuborg** in the command below):

    ```
    sf org login web -d -a myhuborg
    ```

2. Clone the trailhead-dev repository:

    ```
    git clone https://github.com/MkHunter/trailhead-dev
    cd trailhead-dev
    ```

3. Create a scratch org and provide it with an alias (**trailhead-dev** in the command below):

    ```
    sf org create scratch -d -f config/project-scratch-def.json -a trailhead-dev
    ```

4. Push the app to your scratch org:

    ```
    sf project deploy start
    ```

5. Assign the **trailhead** permission set to the default user:

    ```
    sf org assign permset -n trailhead
    ```

6. Import sample data:

    ```
    sf data tree import -p ./data/data-plan.json
    ```

7. Open the scratch org:

    ```
    sf org open
    ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [x] Add README
- [ ] Add badge

See the [open issues](https://github.com/MkHunter/trailhead-dev/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Miguel López [@Trailblazer](https://www.salesforce.com/trailblazer/profile)

Project Link: [https://github.com/MkHunter/trailhead-dev](https://github.com/MkHunter/trailhead-dev)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Resources

* [Apex Code Cheatsheet](https://www.apexhours.com/wp-content/uploads/2023/06/SF_apex_code_cheatsheet_FINAL-1.pdf)

<p align="right">(<a href="#readme-top">back to top</a>)</p>