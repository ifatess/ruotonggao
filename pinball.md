---
layout: blocks
title: Pinball
date: 2020-11-30T16:00:00.000+00:00
page_sections:
- template: navigation-header-w-button
  block: header-2
  logo: "/uploads/2021/01/27/hear.png"
  cta:
    url: "/ruotonggao/photography"
    button_text: Next Project
  navigation: []
- template: navigation-header
  block: header-1
  logo: "/uploads/2021/01/27/bhome.png"
  navigation:
  - link_text: Next Project
    link: "/photography"
- template: hero-banner-w-image
  block: hero-2
  background_image: ''
  image:
    image: "/uploads/2021/01/27/0-5.png"
    alt_text: ''
  content: "<strong>Inspiration<br><br></strong>Inspired by a DIY craft video on Youtube,
    I created a Wi-Fi communication 3D pinball game that was based on Arduino.<br><br><strong>My
    Role<br></strong>Inspiration proposing, programming, UI designing"
  cta:
    enabled: false
    url: ''
    button_text: ''
  headline: <span class="light">Wi-Fi-Based Arduino Pinball Machine Design</span>
- template: 3-column-text
  block: three-column-1
  col_1:
    headline: Step 1
    slug: ''
    content: Design and assemble the playfield
  col_2:
    headline: Step 2
    slug: ''
    content: Establish WIFI communication between server, client and Arduino board
  col_3:
    headline: Step 3
    slug: ''
    content: Program the electronics block. Design an interactive app to control the
      game.
- template: content-feature
  block: feature-1
  media_alignment: Right
  headline: Design the playfield with paper
  content: Borrowing from traditional 3D pinball games, we designed the prototype
    of our game on paper at first. In addition to the bounce zone, I added a special
    bonus area to make the game more innovative and creative.<br><br>I used wooden
    boards, rubber bands, glue, etc. to make a model of a ladder-like slope structure.
  slug: ''
  media:
    image: "/uploads/2021/01/29/5-1.png"
    alt_text: ''
- template: full-width-media-element
  block: media-1
  image: "/uploads/2021/01/29/5-2.png"
  caption: 'Wi-Fi Connection: server, client and Arduino board are connected by Wi-Fi
    established by me'
  slug: ''
- template: 1-column-text
  block: one-column-1
  headline: Arduino Board
  slug: ''
  content: ''
- template: 2-column-media-element
  block: media-2
  image_1:
    image: "/uploads/2021/01/29/5-9.png"
    caption: designing a reasonable circuit
  image_2:
    image: "/uploads/2021/01/29/5-4.png"
    caption: connecting the different parts by wires
- template: detail-content
  block: text-1
  content: "<p><strong>Normal Score:<br></strong>The longer the time between the start
    of the ball and the failure, the higher the score. Controlled by buttons on the
    phone.<br><br><strong>Bonus Score:<br></strong>If the ball and sensor contact
    triggers the sensor, the chip will return the information to the Android terminal,
    the player will get additional bonus rewards. The more you touch the sensor, the
    higher the score.  </p>"
  headline: 'Highlight: Score Section'
- template: 2-column-media-element
  block: media-2
  image_1:
    image: "/uploads/2021/01/29/5-5.png"
    caption: ''
  image_2:
    image: "/uploads/2021/01/29/5-6.gif"
    caption: ''
- template: content-feature
  block: feature-1
  media_alignment: Right
  headline: 'Interactive App: Controller'
  slug: ''
  content: The app is written in Java in Android Studio. After installation, the controller
    can be connected to the server through Wi-Fi.<br><br>It's a one-page controller,
    containing four interactive buttons, a scoring section, a notification bar, and
    connection settings. My classmates understood how to use it at a glance and didn't
    face any problems while interacting with this concise interface.
  media:
    image: "/uploads/2021/01/29/5-7.png"
    alt_text: ''
- template: 1-column-text
  block: one-column-1
  headline: Finished Product
  content: <a href="/ruotonggao/uploads/app-debug.apk" title="app">Click here to download
    the app</a>
  slug: ''
- template: full-width-media-element
  block: media-1
  slug: ''
  image: "/uploads/2021/01/29/5-8.png"
  caption: ''
- template: content-feature
  block: feature-1
  media_alignment: Left
  headline: Gameplay
  slug: ''
  content: Due to the non-instantaneous nature of wifi transmission, it is difficult
    to record the status of the small ball as it is launched and dropped. Therefore,
    I have taken the approach of manually setting the game start and end.<br><br>While
    the game is in progress, the player controls the rise and fall of the pedals and
    tries to get a high score (1. keep the ball on the board as long as possible;
    2. try to get bonuses).
  media:
    image: "/uploads/2021/01/29/5-3.png"
    alt_text: ''
- template: 1-column-text
  block: one-column-1
  headline: Check How it Works!
  slug: ''
  content: ''
- template: full-width-media-element
  block: media-1
  caption: Video
  slug: ''
  image: "/uploads/2020/12/21/pinball.mov"
- template: simple-footer
  block: footer-1
  content: <a href="/ruotonggao/pinball#" title="">Back to Top</a>
menu:
  main:
    weight: 5

---
