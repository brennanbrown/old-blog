---
layout: post
title: My Duck Portfolio
subtitle: Creating my first website from scratch.
date: '2020-06-09T05:13:51.056Z'
author: Brennan K. Brown
permalink: "/my-duck-portfolio/"
image: https://cdn-images-1.medium.com/max/800/1*d0iYiKigZJ-bBSAG7CCcuw.png
image_caption: My workspace during the project, doing remote work.
canonical_url: https://medium.com/@brennanbrown/my-duck-portfolio-eb37faed168d
medium_id: eb37faed168d
---

For the past three weeks, I have built a website from scratch using several different technologies and frameworks. My initial commit to the project’s repository was May 19th, and it was presented on June 8th.

For the front-end, I utilized the [Bootstrap](https://getbootstrap.com/) toolkit and [jQuery](https://jquery.com/) framework in order to have the foundations of a solid, responsive mobile-first design. The rest of the JavaScript is vanilla.

For the back-end, I am using [node.js](https://nodejs.org/en/) with the [Express](https://expressjs.com/) framework on top, as well as [Embedded JavaScript Templating](https://ejs.co/) as my template engine.

Additionally, I am using the NPM packages [ESLint](https://eslint.org/) and [Prettify](https://www.npmjs.com/package/prettify) for code analysis and pattern maintenance, the packages [Mocha](https://mochajs.org/) and [Chai](https://www.chaijs.com/) for testing, and the packages [http-errors](https://www.npmjs.com/package/http-errors) and [body-parser](https://www.npmjs.com/package/body-parser) for validation.

Finally, this website is currently being deployed on [Heroku](https://www.brennanbrown.ca/heroku.com) under a free Dyno plan, so I apologize for any issues regarding speed or connectivity!

![A screenshot of the current state of my website](https://cdn-images-1.medium.com/max/800/1*WZQ1v_sR96XEokUtKxmZXw.png)

Take a look at it here: [https://www.brennanbrown.ca/](https://www.brennanbrown.ca/)

### Why This?

I decided to build my own web portfolio as the subject of this project to further my knowledge regarding back-end web technologies, while creating something that will be beneficial to my career. I hope that this demonstrative, visually-appealing website exemplifies my talents and character, as well as opens up opportunities to network with others.

**Limitations:** Through sheer luck, I managed to get my initial objectives set for this website completed on time, and in a presentable fashion. However, compared to the scope (and importance) of other group’s projects, I feel like there is a lot currently lacking. In theory, an informational website such as this could be displayed completely statically, not requiring such a robust back-end.

If I had extended time, I would have added an actual database component (Eg. MySQL or Redis) instead of simple .JSON files, as well as look into adding an authentication/security page. I would have also liked to have been able to work on more ambitious front-end aspects as well, such as a [Life In Weeks](https://notes.busterbenson.com/life-in-weeks) visualization, or add a preprocessor to my styles such as SASS or LESS.

### Current Pages

Currently, there are three separate pages on this website to demonstrate different features and functionality within the scope of the described framework:

-   [**Docs:**](https://www.brennanbrown.ca/docs) is an example of a static webpage and has the project’s README instructions to download and deploy your own version of this open-sourced website.
-   [**Projects:**](https://www.brennanbrown.ca/project) is an example of a dynamic webpage that parses through a local .JSON file and pulls data to display in HTML.
-   [**Feedback:**](https://www.brennanbrown.ca/feedback) is also an example of a dynamic webpage, however it also allows the client/end-user to add to the local .JSON file, and has proper error-handling and validation of respective input fields.

---

This project is a collaboration between [Duck Labs](http://ducklabs.com/) and [EvolveU](https://www.evolveu.ca/) that aims to teach students the entirety of the spectrum of full-stack web development, starting with the visuals and UX of the front-end, and ending with the database and server communication of the back-end, with the result being a complete and functional website.

Specifically, this work is meant to exemplify the pedagogy of **Project-based Learning**. PBL is an instructional methodology that encourages students to learn and apply knowledge and skills through an engaging experience. PBL presents opportunities for deeper learning in-context and for the development of important skills tied to career readiness.

#### **Why Project-based Learning?**

In essence, the PBL model consists of these seven characteristics:

-   Focuses the student on a big open-ended question, challenge, or problem to research and respond to and/or solve.
-   Brings what students should academically know, understand, and be able to do into the equation.
-   Is inquiry-based.
-   Uses 21st-century skills such as critical thinking, communication, collaboration, and creativity, among others.
-   Builds student choice into the process.
-   Provides opportunities for feedback and revision of the plan and the project.
-   Requires students to present their problems, research process, methods, and results.

---

#### Final Thoughts

I feel as though the learning process was fast-paced and intense, which was very motivating. Having to create something within a deadline like this pushed me to work at the fullest of my potential.

It affected my learning greatly, for the better. There was no time for me to afford to be ambiguous or nebulous, and it really makes you appreciate how much specific programming information is searchable and how many shortcuts are available as well.

The Duck Lab teachers, Sheldon, Chris, and Tony all did excellent jobs at presenting their lessons over the course of the first two weeks. They were extremely helpful and informative and always open for questions on Discord. I really appreciate the fact they tried doing this, and I hope they do it again for the sake of future learners.

For future reference, I would say that you should start as soon as possible, and start small. To me, getting a functioning product somewhere near completed is far more meaningful than just barely getting started on something lofty and ambitious. I would most likely try to work on a team to expand on collaboration and working on project management. If possible, I would also like a few more lessons, though the free week was also very helpful.

In short, learning an entirely new concept and actually using it. Before starting this, I had no prior knowledge of Node.js, and now I can create any sort of website with it. That sort of creative freedom is very powerful, and feels like success. I feel as though I have grown substantially. Seeing my website deploy successfully for the first time after several hours of troubleshooting gave me a sense of confidence and self-worth that I don’t remember feeling before.

---

### Development Documentation

#### Prerequisites

For development, you will only need Node.js and NPM installed in your environement.

If you’re on Windows, go on [official Node.js website](https://nodejs.org/) and download the installer. Also, be sure to have `git` available in your PATH, `npm` might need it (You can find git [here](https://git-scm.com/)).

If you’re on Ubuntu, you can install nodejs and npm easily with apt install, just run the following commands.

`$ sudo apt install nodejs $ sudo apt install npm`

#### Other Operating Systems

You can find more information about the installation on the [official Node.js website](https://nodejs.org/) and the [official NPM website](https://npmjs.org/).

If the installation was successful, you should be able to run the following command.

```
$ node --versionv8.11.3
```
```
$ npm --version6.1.0
```

If you need to update `npm`, you can make it using `npm`! Cool right? After running the following command, just open again the command line and be happy.

```
$ npm install npm -g
```

#### Installation

```
$ git clone https://github.com/brennanbrown/duck-project.git
```
```
$ cd duck-project
```
```
$ npm i
```

#### Running the project:

```
$ npm start
```

Once the server has started up, you can visit it at localhost:3000/, or [127.0.0.1:3000/](https://www.brennanbrown.ca/127.0.0.1:3000/).

#### Roadmap and Contributing

See the [open issues](https://github.com/brennanbrown/duck-project/issues) for a list of proposed features (and known issues).

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

#### License

Distributed under the MIT License. See `LICENSE` for more information.

#### Contact

Brennan K. Brown — [@brennankbrown](https://twitter.com/brennanbrown) — brennankbrown@pm.me

Project Link: [https://github.com/brennanbrown/duck-project](https://github.com/brennanbrown/duck-project)

#### Acknowledgements

-   [README Template](https://github.com/othneildrew/Best-READ.ME-Template)
-   [Logo Source](https://commons.wikimedia.org/wiki/File:Duck_Sotka1.svg)
-   [Prettify](https://www.npmjs.com/package/prettify)
-   [ESLint](https://eslint.org/)
-   [auto0 .gitignore](https://gist.github.com/dan-auth0/2fb996dc8080eaae0900100bf1c3fa26)
-   [Favicon.io](https://favicon.io/)
-   [Img Shields](https://shields.io)
-   [Choose an Open Source License](https://choosealicense.com)
-   [GitHub Pages](https://pages.github.com)
