"parts": [
    {
      "type": "wokwi-arduino-uno",
      "id": "uno",
      "top": 61.86,
      "left": -3.73,
      "rotate": 180,
      "attrs": {}
    },
    {
      "type": "wokwi-resistor",
      "id": "r1",
      "top": -37.43,
      "left": 132.43,
      "rotate": 90,
      "attrs": { "value": "1000" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r2",
      "top": -37.3,
      "left": 96.64,
      "rotate": 90,
      "attrs": { "value": "1000" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r3",
      "top": -34.77,
      "left": 51.01,
      "rotate": 90,
      "attrs": { "value": "1000" }
    },
    {
      "type": "wokwi-resistor",
      "id": "r11",
      "top": 378.54,
      "left": 187.02,
      "rotate": 90,
      "attrs": { "value": "1000" }
    },
    {
      "type": "wokwi-rgb-led",
      "id": "rgb1",
      "top": -165.3,
      "left": 84.17,
      "attrs": { "common": "cathode" }
    },
    {
      "type": "wokwi-pushbutton",
      "id": "btn4",
      "top": 438.13,
      "left": 148.01,
      "attrs": { "color": "green" }
    }
  ],
  "connections": [
    [ "rgb1:R", "r3:1", "green", [ "v1.06", "h-19.21" ] ],
    [ "rgb1:G", "r2:1", "green", [ "v16.29", "h12.17" ] ],
    [ "rgb1:B", "r1:1", "green", [ "v16.32", "h37.68" ] ],
    [ "uno:GND.2", "rgb1:COM", "black", [ "v-177.12", "h7.06" ] ],
    [ "r3:2", "uno:9", "green", [ "h0.43", "v57.83", "h193.63", "v212.65", "h-173.48" ] ],
    [ "r2:2", "uno:10", "green", [ "h-0.93", "v58.74", "h148.86", "v220.49", "h-151.1" ] ],
    [ "r1:2", "uno:11", "green", [ "h0.12", "v62.25", "h113.72", "v223.85", "h-147.24" ] ],
    [ "uno:GND.1", "r11:1", "black", [ "v32.68", "h57.13" ] ],
    [ "r11:2", "btn4:1.r", "black", [ "h-0.95", "v25.87" ] ],
    [ "btn4:1.l", "uno:5", "green", [ "h-8.63", "v-168.54", "h-82.55" ] ],
    [ "uno:5V", "btn4:2.r", "red", [ "v-13.11", "h170.8", "v229.06", "h-55.81", "v180.23" ] ]
  ]
}
