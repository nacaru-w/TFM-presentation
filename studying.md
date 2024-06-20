---
title: "<span class='container'><img style='max-width: 3em;' src='./img/UOC_logo.svg' /></span><br/><span style='font-size: 0.8em;'>Web and back-end utilities for Wikipedia<span>"
author: <a href="https://es.wikipedia.org/wiki/Usuario:Nacaru">Nacho Casares</a>
lang: es
theme: white
title-slide-attributes:
    data-background-image: "./img/HD-hotspot-bg.png"
css: ["custom.css"]
width: 1024
height: 768
margin: 0.02
slideNumber: true
showNotes: true
history: true
transitionSpeed: fast
---

<div style="font-size:1.2em">
[`https://nacaru-w.github.io/memoria/memoria.pdf`](https://nacaru-w.github.io/memoria/memoria.pdf)
</div>

# Introduction {data-background-image="img/Elegant_Background-2.jpg"}
![](./img/Wikipedia%20logo%20version%202.svg){ width=200px }

***

- Wikipedia: free encyclopedia that anyone can edit
- Depends on volunteer contributions, mostly
- Low number of technical contributors
- High demand for this kind of support
 
# Objectives {data-background-image="img/Elegant_Background-3.jpg"}

***

- To provide the Spanish Wikipedia with a community-supported bot that applies MoS rules
- To build a website that the LGBT+ WikiProject can use to display their work, common goals and achievements.

# Context and justification {data-background-image="img/Elegant_Background-7.jpg"}

## Bot

- Users invest a significant amount of time applying Manual of Style (MoS) rules.
- Many of these rules can be applied automatically through technical means.
- Less time dedicated to implementing MoS means more time creating content → primary goal of the encyclopedia

## LGBT+ WikiProject website

- Group of users dedicated to improving LGBT+ content on the Spanish Wikipedia
- Low amount of technical editors among them
- Other user groups already have their own webpage

# LGBT+ WikiProject website {data-background-color="aliceblue"}
![](./img/barba.svg){ width=200px }

***

[https://wmlgbt-es-web.toolforge.org](https://wmlgbt-es-web.toolforge.org)

***

[https://github.com/nacaru-w/WikiprojectLGBT-Webpage](https://github.com/nacaru-w/WikiprojectLGBT-Webpage)

## Design: web neobrutalism {data-background-color="whitesmoke"}

![](./img/main_page_screenshot.png)

***
## {data-background-color="whitesmoke"}

![](./img/blog_element.png){width=16em}

***
## {data-background-color="whitesmoke"}

![](./img/guitar_element.png){width=18em}

***
## {data-background-color="whitesmoke"}

![](./img/graph_element.png){width=16em}

## Characteristics

- Built using [Angular 17.3](https://angular.dev/)
- Single-page application (SPA)
- Smooth transitions

## Technologies

- Uses [Bootstrap](https://getbootstrap.com/)
- Hosted in [Toolforge](https://admin.toolforge.org/)
- Interacts with [MediaWiki API](https://www.mediawiki.org/wiki/API:Main_page)
- Has its own database ([MariaDB](https://mariadb.org/))
- Authentication via [MediaWiki OAuth](https://www.mediawiki.org/wiki/OAuth/For_Developers)
- Uses [Angular Animations](https://www.npmjs.com/package/@angular/animations)

## Architecture

![](./img/lgbt_website_architecture_new.png)

## Blog component

![](./img/blog_component.png){width=16em}

## Stats component

![](./img/stats_component.png){width=16em}

## Form component

![](./img/form_component.png){width=16em}

## Blog admin panel component

![](./img/blog_admin_panel.png){width=16em}

## Blog edit component

![](./img/blog_edit_component.png){width=16em}

## API interactions

![](./img/api_interactions.png){width=18em}

# Manual of Style Bot {data-background-color="lightgray"}
![](./img/cyan-bot.svg)

***

[https://es.wikipedia.org/wiki/Usuario:NacaruBot](https://es.wikipedia.org/wiki/Usuario:NacaruBot)

***

[https://github.com/nacaru-w/NacaruBot](https://github.com/nacaru-w/NacaruBot)

## Asking for permission

Bots need community authorisation first
![](./img/bot_development_cycle.png)

## Technologies

- Uses [node.js](https://nodejs.org/en)
- Uses [mwn](https://www.npmjs.com/package/mwn), a comprehensive bot framework
- Written in TypeScript
- Interacts through the [MediaWiki API](https://www.mediawiki.org/wiki/API:Main_page)
- Thorough log of all the actions

## Architecture

![](./img/bot_architecture.png)

## Action

The bot erases links to internal dates in articles that are not related to the calendar

![](./img/bot_diff_screenshot.png)

## Log

It logs every action it carries out

![](./img/bot.png)

***

Log is also visible on Wikipedia
![](./img/bot_action_contribs.png)

# Fin {data-background-image="./img/Back3.png"}