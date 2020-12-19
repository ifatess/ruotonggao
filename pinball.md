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
    content: Program the electronics block and debug
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
  content: <h4>1. Connect Arduino Board and ESP8266 with wires;</h4><h4>2. Establish
    TCP connection;</h4><p>AT+CIPSTART=0,"TCP","192.168.4.1",5000 //connect</p><p>AT+CIPSEND=0,4
    //confirm</p><p>length sent //send messege</p><h4>3. Receive order from server.</h4><p>if(Serial.available()){</p><p>wifi.write(Serial.read());}</p><p></p><p>order=readTtl();</p><p>if(order!=""){</p><p>order.trim();</p><p>wifi.println(order);</p><p>Serial.print(order);}</p><p></p><p>String
    wifidata=getWifiSerialData();</p><p>if(wifidata!=""){</p><p>Serial.println(wifidata);}</p><p>...</p>
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
    the different parts by wires and designing a reasonable circuit.
menu:
  main:
    weight: 5

---
