# TiberiusHunter's Home Assistant Configuration

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

![Project Maintenance][maintenance-shield]
[![MIT License][license-shield]][license-url]

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

<!-- ABOUT -->
## About

A repository storing and backing up my Home Assistant configuration

<!-- FILE STRUCTURE -->
## File Structure

The entry point for Home Assistant is the `configuration.yaml` file. From there I've split up the configuration into various folders and files found under the `/configuration/` directory.

This has simply been to reduce the size of the `configuration.yaml` *especially as my previous installation of Home Assistant ended up being a nightmare to maintain..* :roll_eyes:

From the `configuration.yaml` file, all the files under the `configuration/integrations/` directory get imported - this lists what you'd likely see in a regular configuration file.

Once an integration contains any entities, sensors, scenes, scripts, etc. I then break that down into it's own file under whichever type of integration it is - For example, for the `camera:` integration I've created a separate file under `configuration/entities/camera/` directory for each camera.

<!-- USAGE -->
## Usage

This repository has been designed to be used with the default [git pull addon][addon-git-pull] once the build passes on the main branch.

When there are changes to any of the configuration files Home Assistant will pull the latest changes and automatically restart :tada:

<!-- CONTRIBUTING -->
## Contributing

You've found a bug in my config, a mistake in the docs or maybe you want to add a new feature? :thinking:

I'm very open to any and all contributions to my config, please let me know by creating an [issue on the repository][issues-url] and feel free to create a pull request with your changes :heart:

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->
## License

Distributed under the MIT License. See [LICENSE][license-url] for more information.

<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* [rxaiver's GitHub Emoji Cheat Sheet][1]
* [Img Shields][2]
* [Choose an Open Source License][3]
* [othneildrew's Best README Template][4]
* [Frenck's Home Assistant Config][5]

<!-- CONTACT -->
## Contact

Owner: Sam Welek

[![GitHub][github-shield]][github-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
[![X][x-shield]][x-url]

<a href="https://www.buymeacoffee.com/tiberiushunter" target="_blank"> <img src="https://cdn.buymeacoffee.com/buttons/default-yellow.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Project Link: [GitHub][project-url]

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

<!-- Project Specific -->
[project-url]: https://github.com/tiberiushunter/hassio-config/

[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg?style=for-the-badge

[contributors-shield]: https://img.shields.io/github/contributors/tiberiushunter/hassio-config.svg?style=for-the-badge
[contributors-url]: https://github.com/tiberiushunter/hassio-config/graphs/contributors

[forks-shield]: https://img.shields.io/github/forks/tiberiushunter/hassio-config.svg?style=for-the-badge
[forks-url]: https://github.com/tiberiushunter/hassio-config/network/members

[stars-shield]: https://img.shields.io/github/stars/tiberiushunter/hassio-config.svg?style=for-the-badge
[stars-url]: https://github.com/tiberiushunter/hassio-config/stargazers

[issues-shield]: https://img.shields.io/github/issues/tiberiushunter/hassio-config.svg?style=for-the-badge
[issues-url]: https://github.com/tiberiushunter/hassio-config/issues

[license-shield]: https://img.shields.io/github/license/tiberiushunter/hassio-config.svg?style=for-the-badge
[license-url]: https://github.com/tiberiushunter/hassio-config/blob/main/LICENSE

[addon-git-pull]: https://github.com/home-assistant/hassio-addons/tree/master/git_pull

<!-- Contact Specific -->
[github-shield]: https://img.shields.io/badge/-GitHub-black.svg?style=for-the-badge&logo=github&colorB=555
[github-url]: https://github.com/tiberiushunter

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/sam-welek

[x-shield]: https://img.shields.io/badge/-X-black.svg?style=for-the-badge&logo=x&colorB=555
[x-url]: https://x.com/samwelek

<!-- Acknowledgement Specific -->
[1]: https://gist.github.com/rxaviers/7360908
[2]: https://shields.io
[3]: https://choosealicense.com
[4]: https://github.com/othneildrew/Best-README-Template
[5]: https://github.com/frenck/home-assistant-config
