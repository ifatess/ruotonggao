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
  headline: Connection
  content: "<ol><li><p>Connect Arduino Board and ESP8266 with wires;</p></li><li><p>Establish
    TCP connection</p><pre><code>AT+CIPSTART=0,\"TCP\",\"192.168.4.1\",5000 //connect\nAT+CIPSEND=0,4
    //confirm length\nsent //send messege</code></pre></li><li><p>Receive order from
    server</p><pre><code>if(Serial.available()){\n\twifi.write(Serial.read());\n}\n\norder=readTtl();\nif(order!=\"\"){\n\torder.trim();\n\twifi.println(order);\n\tSerial.print(order);}\n\nString
    wifidata=getWifiSerialData();\n\tif(wifidata!=\"\"){\n\tSerial.println(wifidata);\n}\n\n...</code></pre></li></ol>"
menu:
  main:
    weight: 5

---
