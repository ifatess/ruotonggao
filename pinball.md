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
  content: "<h5>1. Connect Arduino Board and ESP8266 with wires;</h5><h5>2. Establish
    TCP connection;</h5><blockquote><p>AT+CIPSTART=0,\"TCP\",\"192.168.4.1\",5000
    //connect\r\nAT+CIPSEND=0,4 //confirm length\r\nsent //send messege</p></blockquote><h5>3.
    Receive order from server.</h5><blockquote><p>if(Serial.available()){\r\n\twifi.write(Serial.read());\r\n}\r\n\r\norder=readTtl();\r\nif(order!=\"\"){\r\n\torder.trim();\r\n\twifi.println(order);\r\n\tSerial.print(order);}\r\n\r\nString
    wifidata=getWifiSerialData();\r\n\tif(wifidata!=\"\"){\r\n\tSerial.println(wifidata);\r\n}\r\n\r\n...</p></blockquote>"
menu:
  main:
    weight: 5

---
