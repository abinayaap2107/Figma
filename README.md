# Ex08 Event Registration Web Application
## Date:19.3.2026

## AIM:
To design, develop and deploy a web application for event registration using Figma UI tool.

## UI DESIGN TOOL:
Figma

## DESIGN STEPS:

### Step 1:
Use frames to represent screens or sections.

### Step 2:
Add column grids for consistent spacing and alignment.

### Step 3:
Insert shapes, text, buttons, and icons.

### Step 4:
Use Auto Layout for flexible, responsive design.

### Step 5:
Define color, text, and effect styles globally for consistency.

### Step 6:
Name layers logically and group related elements.

### Step 6:
Link frames to show navigation or interactions.

### Step 7:
Select the specific frame while generating code using Anima plugin.

## CODE:
page1 
index.html
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <img class="bg" src="img/bg-1.png" />
      <img class="logo" src="img/logo.png" />
      <img class="download" src="img/download-2-1.png" />
      <div class="text-wrapper">SPORTS DAY EVENTS</div>
      <div class="rectangle"></div>
      <div class="div"></div>
      <div class="text-wrapper-2">Login</div>
      <div class="text-wrapper-3">Register</div>
    </div>
  </body>
</html>

```
global.css
```
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}

```
style.css
```
.android-compact {
  background-color: #ffffff;
  width: 100%;
  min-width: 412px;
  min-height: 917px;
  position: relative;
}

.android-compact .bg {
  position: absolute;
  top: 1px;
  left: 0;
  width: 412px;
  height: 916px;
  aspect-ratio: 1.6;
  object-fit: cover;
}

.android-compact .logo {
  position: absolute;
  top: 28px;
  left: 0;
  width: 412px;
  height: 84px;
  aspect-ratio: 5.01;
  object-fit: cover;
}

.android-compact .download {
  position: absolute;
  top: 147px;
  left: 116px;
  width: 178px;
  height: 171px;
  aspect-ratio: 1.04;
  object-fit: cover;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 395px;
  left: 31px;
  width: 350px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #1451c1;
  font-size: 32px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .rectangle {
  top: 581px;
  box-shadow: 0px 4px 4px #00000040;
  position: absolute;
  left: 97px;
  width: 197px;
  height: 49px;
  background-color: #654bcd;
}

.android-compact .div {
  top: 665px;
  position: absolute;
  left: 97px;
  width: 197px;
  height: 49px;
  background-color: #654bcd;
}

.android-compact .text-wrapper-2 {
  position: absolute;
  top: 594px;
  left: 168px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 20px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.android-compact .text-wrapper-3 {
  position: absolute;
  top: 678px;
  left: 154px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 20px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

```
page3
index.html
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-medium">
      <img class="images" src="img/images-1.png" />
      <div class="text-wrapper">Event Registration Form</div>
      <div class="rectangle"></div>
      <div class="div"></div>
      <div class="rectangle-2"></div>
      <div class="rectangle-3"></div>
      <div class="rectangle-4"></div>
      <div class="rectangle-5"></div>
      <div class="rectangle-6"></div>
      <div class="rectangle-7"></div>
      <div class="text-wrapper-2">Full Name</div>
      <div class="text-wrapper-3">Gender</div>
      <div class="text-wrapper-4">Age</div>
      <div class="text-wrapper-5">Register Number</div>
      <div class="text-wrapper-6">Department</div>
      <div class="text-wrapper-7">Mobile Number</div>
      <div class="text-wrapper-8">Email ID</div>
      <div class="text-wrapper-9">Events to Register</div>
      <div class="rectangle-8"></div>
      <div class="text-wrapper-10">Register</div>
    </div>
  </body>
</html>

```
globals.css
```
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Black", "weight": "900", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Black";
  src: local("Inter-Black");
}

```
style.css
```
.android-medium {
  background-color: #ffffff;
  width: 100%;
  min-width: 412px;
  min-height: 917px;
  position: relative;
}

.android-medium .images {
  position: absolute;
  top: 0;
  left: 0;
  width: 412px;
  height: 917px;
  aspect-ratio: 0.56;
  object-fit: cover;
}

.android-medium .text-wrapper {
  position: absolute;
  top: 57px;
  left: 51px;
  width: 317px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #195c77;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .rectangle {
  position: absolute;
  top: 174px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .div {
  position: absolute;
  top: 676px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .rectangle-2 {
  position: absolute;
  top: 608px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .rectangle-3 {
  position: absolute;
  top: 540px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .rectangle-4 {
  position: absolute;
  top: 242px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .rectangle-5 {
  position: absolute;
  top: 310px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .rectangle-6 {
  position: absolute;
  top: 378px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .rectangle-7 {
  position: absolute;
  top: 459px;
  left: 26px;
  width: 232px;
  height: 34px;
  background-color: #d9d9d933;
  box-shadow: inset 0px 4px 4px #00000040;
}

.android-medium .text-wrapper-2 {
  position: absolute;
  top: 187px;
  left: 69px;
  width: 74px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 15px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper-3 {
  position: absolute;
  top: 250px;
  left: 51px;
  width: 80px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 14px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper-4 {
  position: absolute;
  top: 318px;
  left: 54px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 14px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper-5 {
  position: absolute;
  top: 381px;
  left: 46px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 14px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper-6 {
  position: absolute;
  top: 467px;
  left: 46px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 14px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper-7 {
  position: absolute;
  top: 548px;
  left: 46px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 14px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper-8 {
  position: absolute;
  top: 616px;
  left: 51px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 14px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .text-wrapper-9 {
  position: absolute;
  top: 688px;
  left: 42px;
  font-family: "Inter-Black", Helvetica;
  font-weight: 900;
  color: #000000;
  font-size: 14px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-medium .rectangle-8 {
  position: absolute;
  top: 756px;
  left: 134px;
  width: 159px;
  height: 41px;
  background-color: #d1318c;
}

.android-medium .text-wrapper-10 {
  position: absolute;
  top: 765px;
  left: 172px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 20px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

```
page 2
index.html
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <img class="img" src="img/bec57db7a674c518093900cf974657ff-1.png" />
      <div class="text-wrapper">Sports Day Events</div>
      <div class="div">CRICKET</div>
      <div class="text-wrapper-2">BADMINTON</div>
      <div class="text-wrapper-3">THROW BALL</div>
      <div class="text-wrapper-4">100 M</div>
      <div class="text-wrapper-5">200 M</div>
      <div class="text-wrapper-6">4*100 M RELAY</div>
    </div>
  </body>
</html>

```
globals.css
```
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}

```
style.css
```
.android-compact {
  background-color: #ffffff;
  width: 100%;
  min-width: 412px;
  min-height: 917px;
  position: relative;
}

.android-compact .img {
  position: absolute;
  top: 0;
  left: 0;
  width: 412px;
  height: 917px;
  aspect-ratio: 1.42;
  object-fit: cover;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 91px;
  left: 71px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #7f32b2;
  font-size: 30px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
  white-space: nowrap;
}

.android-compact .div {
  position: absolute;
  top: 225px;
  left: 41px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #b93493;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-2 {
  position: absolute;
  top: 285px;
  left: 41px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #b93494;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-3 {
  position: absolute;
  top: 345px;
  left: 41px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #b93494;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-4 {
  position: absolute;
  top: 405px;
  left: 41px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #b93494;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-5 {
  position: absolute;
  top: 459px;
  left: 41px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #b93494;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-6 {
  position: absolute;
  top: 513px;
  left: 41px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #b93494;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

```
page 4
index.html
```
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <img class="download" src="img/download-3-1.png" />
      <img class="logo" src="img/logo-1.png" />
      <div class="text-wrapper">Thanks for Registering</div>
      <div class="contact-us-e-mail">
        Contact Us:<br />E-Mail:<br />sportsevents@saveetha.ac.in<br />Phone:<br />9456312810
      </div>
    </div>
  </body>
</html>

```
globals.css
```
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}

```
style.css
```
.android-compact {
  background-color: #ffffff;
  width: 100%;
  min-width: 412px;
  min-height: 917px;
  position: relative;
}

.android-compact .download {
  position: absolute;
  top: 0;
  left: 0;
  width: 412px;
  height: 917px;
  aspect-ratio: 1.82;
  object-fit: cover;
}

.android-compact .logo {
  position: absolute;
  top: 48px;
  left: 0;
  width: 412px;
  height: 86px;
  aspect-ratio: 5.01;
  object-fit: cover;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 359px;
  left: 10px;
  width: 391px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #23a083;
  font-size: 34px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .contact-us-e-mail {
  position: absolute;
  top: 727px;
  left: 10px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #062d35;
  font-size: 24px;
  text-align: center;
  letter-spacing: 0;
  line-height: normal;
}

```
## OUTPUT:
<img width="1920" height="1080" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/27bec480-46d9-49ff-9b38-382fad478ca4" />
<img width="1920" height="1080" alt="Screenshot (76)" src="https://github.com/user-attachments/assets/db31adef-4fcf-4e08-8ff9-c691e5d6bea7" />
<img width="1920" height="1080" alt="Screenshot (77)" src="https://github.com/user-attachments/assets/313d5671-b784-4546-bd97-bc887a73169f" />
<img width="1920" height="1080" alt="Screenshot (78)" src="https://github.com/user-attachments/assets/6a12972d-fc62-478b-8fb7-48517695b109" />






## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
