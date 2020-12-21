---
layout: blocks
title: Pinball
date: 2020-11-30T16:00:00.000+00:00
page_sections:
- template: navigation-header
  block: header-1
  logo: "/uploads/2020/12/04/1.png"
  navigation:
  - link: "/photography"
    link_text: Next Project
- template: hero-banner-w-image
  block: hero-2
  background_image: "/uploads/2018/06/21/hero-2-bg.png"
  image:
    image: ''
    alt_text: ''
  content: "<strong>Inspiration<br><br></strong>Inspired by a DIY craft video on Youtube,
    I created a Wi-Fi communication 3D pinball game that was based on Arduino."
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
  content: Use wooden boards, rubber bands, glue, etc. to make a model of a ladder-like
    slope structure
  slug: ''
  media:
    image: "/uploads/2020/12/19/32.png"
    alt_text: ''
- template: detail-content
  block: text-1
  headline: Wi-Fi Connection
  content: |-
    <h4>1. Connect Arduino Board and ESP8266 with wires;</h4><p></p><h4>2. Establish TCP connection;</h4><pre><code>AT+CIPSTART=0,"TCP","192.168.4.1",5000 //connect
    AT+CIPSEND=0,4 //confirm length
    sent //send messege</code></pre><h4>3. Receive order from server.</h4><pre><code>order=readTtl();
    if(order!=""){
    order.trim();
    wifi.println(order);
    Serial.print(order);}
    ...</code></pre>
- template: content-feature
  block: feature-1
  media_alignment: Left
  media:
    image: "/uploads/2020/12/19/33.png"
    alt_text: ''
  headline: Develop the Arduino Board
  slug: ''
  content: The task of controlling the servo, establishing communication, and adding
    points through the photosensitive sensor on the Arduino board requires connecting
    the different parts by wires and designing a reasonable circuit.<br><br>Two drivers,
    a photosensitive sensor, and an ESP8266 board (containing a Wi-Fi module) were
    attached to the Arduino board.
- template: content-feature
  block: feature-1
  media_alignment: Right
  headline: 'Highlight: Score Section'
  content: "<strong>Normal Score:<br></strong>The longer the time between the start
    of the ball and the failure, the higher the score. Controlled by buttons on the
    phone.<br><br><strong>Bonus Score:<br></strong>If the ball and sensor contact
    triggers the sensor, the chip will return the information to the Android terminal,
    the player will get additional bonus rewards. The more you touch the sensor, the
    higher the score."
  media:
    image: "/uploads/2020/12/19/34.png"
    alt_text: ''
  slug: ''
- template: full-width-media-element
  block: media-1
  image: "/uploads/2020/12/21/pinball3.gif"
  caption: Preview of the procedure
  slug: ''
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
    image: "/uploads/2020/12/21/35.png"
    alt_text: ''
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
    image: "/uploads/2020/12/21/36.svg"
    alt_text: ''
- template: full-width-media-element
  block: media-1
  caption: Video
  slug: ''
  image: ''
menu:
  main:
    weight: 5

---
