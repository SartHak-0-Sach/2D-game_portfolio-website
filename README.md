# Gamified developer portfolio website

## Welcome! 👋

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [How to setup the project](#how-to-setup-the-project)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [How to run](#how-to-run)
- [How to build](#how-to-build)
- [How to preview the build](#how-to-preview-the-build)
- [How to host](#how-to-host)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- Explore a 2D game environment that serves as a portfolio website.
- Interact with objects like a degree on the wall and a resume on the table.
- Experience the site seamlessly on both desktop and mobile devices.

### How to setup the project

To set up the project locally, follow these steps:

1. Clone the repository using GitHub Desktop or Git Bash:
   ```bash
   git clone https://github.com/SartHak-0-Sach/2D-game_portfolio-website.git
   ```
2. Navigate to the project directory:
   ```bash
   cd 2D-game_portfolio-website
   ```

### Screenshot

![Screenshot](./developerportfoliothumbnail.png)

### Links

- Solution URL: [Link to this repo](https://github.com/SartHak-0-Sach/2D-game_portfolio-website)
- Live Site URL: [Live site URL](https://2-d-game-portfolio-website.vercel.app/)

## How to run

Note: You need Node.js and npm installed on your machine.

```bash
npm install
npm run dev
```

## How to build

```bash
npm run build
```

A `dist` folder should be created.

## How to preview the build

```bash
npm run preview
```

## How to host

Here is a guide: [How to deploy the project](https://github.com/SartHak-0-Sach/2D-game_portfolio-website/blob/main/HOW_TO_DEPLOY.MD)

## My process

### Built with

- KaboomJS
- CSS
- Vite
- Canvas
- HTML

### What I learned

Working on this project allowed me to learn and implement game development concepts using KaboomJS, and also enhanced my skills in creating interactive and responsive web designs.

This project helped me apply all of my JavaScript knowledge into game development, huge shoutout to awesome creators from freecodecamp who illustrate the tutorials so well. Following code snippet is one such example of using basic JS code application into game dev principles-

```js
for (const layer of layers) {
    if (layer.name === "boundaries") {
      for (const boundary of layer.objects) {
        map.add([
          k.area({
            shape: new k.Rect(k.vec2(0), boundary.width, boundary.height),
          }),
          k.body({ isStatic: true }),
          k.pos(boundary.x, boundary.y),
          boundary.name,
        ]);

        if (boundary.name) {
          player.onCollide(boundary.name, () => {
            player.isInDialogue = true;
            displayDialogue(
              dialogueData[boundary.name],
              () => (player.isInDialogue = false)
            );
          });
        }
      }

      continue;
    }
```

### Continued development

I plan to further develop my skills in game development and explore more advanced features of KaboomJS. Additionally, I aim to integrate more interactive elements into my web projects to make them engaging and fun for users.

### Useful resources

- [KaboomJS Documentation](https://kaboomjs.com/) - This is a great resource to learn KaboomJS.
- [MDN Web Docs](https://developer.mozilla.org/) - Comprehensive resource for HTML, CSS, and JavaScript documentation.

## Author

<b><strong>Sarthak Sachdev</strong></b>
- Website - [Sarthak Sachdev](https://itsmesarthak.netlify.app/)
- LeetCode - [@sarthak_sachdev](https://leetcode.com/u/sarthak_sachdev/)
- Twitter - [@sarthak_sach69](https://www.twitter.com/sarthak_sach69)

## Acknowledgments

Special thanks to the vast knowledge base available on YouTube and Stack Overflow, where I learned many of the concepts and got my doubts cleared.

## Got feedback for me?

I love receiving feedback! I am always looking to improve my code and take up new innovative ideas to work upon. So if you have anything you'd like to mention, please email 'hi' at saarsaach30[at]gmail[dot]com.

If you liked this project, make sure to spread the word and share it with all your friends.

**Happy coding!** ☺️🚀
