KnobMan3D
=========

Knob Image Design Tool

KnobMan3D is a Knob Image (film-strip) design tool based on WebGL + THREE.js

* Create your own knobs by combination of basic objects
* Animation effects available
* Rendered image can be exported as PNG file

[Sample 1](http://g200kg.github.io/knobman3d/?d=eyJjYW15IjoiLTczIiwid2lkdGgiOjY0LCJoZWlnaHQiOjY0LCJmcmFtZXMiOjE3LCJsYXllciI6W3sibmFtZSI6Ik9iajEiLCJwcmltIjp7InR5cGUiOiJjeWxpbmRlciIsInNtb290aCI6MTAwLCJoZWlnaHQiOjEwLCJzaGluaW5lc3MiOjQsInRleHR1cmUiOiJQbGFudCIsInRleGRlcHRoIjotMTgsInRleHpvb20iOjI2LCJjb2xvciI6MTU5MDY5NjF9LCJlZmYiOnsib2Zmc2V0eDEiOi0zOCwib2Zmc2V0eTEiOjQwLCJhbmdsZTEiOi03NiwiYW5nbGUyIjo5MSwiYW5nbGVhIjoiMCJ9fSx7Im5hbWUiOiJPYmoyIiwicHJpbSI6eyJ0eXBlIjoiY3lsaW5kZXIiLCJkZWZsYXRlIjozMCwic21vb3RoIjozMiwiaGVpZ2h0IjozMSwidGV4dHVyZSI6IkF1cmEiLCJjb2xvciI6ODA4MTQ2M30sImVmZiI6eyJ6b29teDEiOjU3LCJvZmZzZXR4MSI6LTM0LCJvZmZzZXR5MSI6LTUxLCJhbmdsZTEiOi03MiwiYW5nbGVhIjoiMCJ9fSx7Im5hbWUiOiJPYmozIiwicHJpbSI6eyJ0eXBlIjoiY3ViZSIsInJvdW5kIjoyNiwic21vb3RoIjoyMCwiaGVpZ2h0IjozMCwidGV4dHVyZSI6IlNhbmQiLCJ0ZXhkZXB0aCI6MTEsInRleHpvb20iOjIwMCwiY29sb3IiOjk4NzAxMjl9LCJlZmYiOnsiem9vbXgxIjo0NSwib2Zmc2V0eTEiOjQ5LCJhbmdsZTEiOi0yMywiYW5nbGUyIjoxMzcsImFuZ2xlYSI6IjAifX1dfQ==)  
[Sample 2](http://g200kg.github.io/knobman3d/?d=eyJjYW15IjoiLTMxIiwiY2Ftem9vbSI6MTQzLCJ3aWR0aCI6NjQsImhlaWdodCI6NjQsImZyYW1lcyI6MTcsImxheWVyIjpbeyJuYW1lIjoiT2JqMSIsInByaW0iOnsidHlwZSI6ImN5bGluZGVyIiwid2F2ZSI6Nywid2F2ZWFuZ2xlIjo3LCJzbW9vdGgiOjQ2LCJoZWlnaHQiOjM4LCJzaGluaW5lc3MiOjIyLCJ0ZXh0dXJlIjoiQXVyYSIsImNvbG9yIjoyNjMxNjl9LCJlZmYiOnsiem9vbXgxIjoxMTYsImFuZ2xlMSI6LTE0NSwiYW5nbGUyIjoxNDUsImFuZ2xlYSI6IjAifX0seyJuYW1lIjoiT2JqMiIsInByaW0iOnsidHlwZSI6ImN5bGluZGVyIiwic21vb3RoIjozNiwiaGVpZ2h0Ijo0NSwic2hpbmluZXNzIjoxMCwidGV4dHVyZSI6IlNhbmQiLCJ0ZXhkZXB0aCI6MywiY29sb3IiOjY1NzkyfSwiZWZmIjp7ImFuZ2xlMSI6LTE0NSwiYW5nbGUyIjoxNDUsImFuZ2xlYSI6IjAifX0seyJuYW1lIjoiT2JqMyIsInByaW0iOnsidHlwZSI6ImN1YmUiLCJhc3BlY3QiOjczLCJyb3VuZCI6MzUsInNtb290aCI6ODksImhlaWdodCI6NDgsInNoaW5pbmVzcyI6MTYxLCJ0ZXh0dXJlIjoiQXVyYSIsImNvbG9yIjoxNjcxMTQxNX0sImVmZiI6eyJ6b29teDEiOjY0LCJvZmZzZXR5MSI6MjMsImFuZ2xlMSI6LTE0NSwiYW5nbGUyIjoxNDUsImFuZ2xlYSI6IjAifX1dfQ==)  
[Sample 3](eyJjYW15IjoiLTMxIiwiY2Ftem9vbSI6MTQzLCJ3aWR0aCI6NjQsImhlaWdodCI6NjQsImZyYW1lcyI6MTcsImxheWVyIjpbeyJuYW1lIjoiT2JqMSIsInByaW0iOnsidHlwZSI6ImN5bGluZGVyIiwid2F2ZSI6Nywid2F2ZWFuZ2xlIjo3LCJzbW9vdGgiOjQ2LCJoZWlnaHQiOjM4LCJzaGluaW5lc3MiOjIyLCJ0ZXh0dXJlIjoiQXVyYSIsImNvbG9yIjoyNjMxNjl9LCJlZmYiOnsiem9vbXgxIjoxMTYsImFuZ2xlMSI6LTE0NSwiYW5nbGUyIjoxNDUsImFuZ2xlYSI6IjAifX0seyJuYW1lIjoiT2JqMiIsInByaW0iOnsidHlwZSI6ImN5bGluZGVyIiwic21vb3RoIjozNiwiaGVpZ2h0Ijo0NSwic2hpbmluZXNzIjoxMCwidGV4dHVyZSI6IlNhbmQiLCJ0ZXhkZXB0aCI6MywiY29sb3IiOjY1NzkyfSwiZWZmIjp7ImFuZ2xlMSI6LTE0NSwiYW5nbGUyIjoxNDUsImFuZ2xlYSI6IjAifX0seyJuYW1lIjoiT2JqMyIsInByaW0iOnsidHlwZSI6ImN1YmUiLCJhc3BlY3QiOjczLCJyb3VuZCI6MzUsInNtb290aCI6ODksImhlaWdodCI6NDgsInNoaW5pbmVzcyI6MTYxLCJ0ZXh0dXJlIjoiQXVyYSIsImNvbG9yIjoxNjcxMTQxNX0sImVmZiI6eyJ6b29teDEiOjY0LCJvZmZzZXR5MSI6MjMsImFuZ2xlMSI6LTE0NSwiYW5nbGUyIjoxNDUsImFuZ2xlYSI6IjAifX1dfQ)

![](images/sample1.png) ![](images/sample2.png) ![](images/sample3.png)


Available at :
  [http://g200kg.github.io/knobman3d/](http://g200kg.github.io/knobman3d/)
