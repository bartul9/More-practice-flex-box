
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="styles.css" />
    <title>Flex Box practice</title>
  </head>
  <body><nav><ul>
      <li><a href="">Menu</a></li>
      <li><a href="">About Us</a></li>
      <li id="contact" ><a  href="">Contact</a></li>
  </ul></nav>
    <header> <h1>Cho's Cuisine</h1></header><h2>Today Specialties</h2>
    <div class="container">
       
      <div class="bigbox one">
        <div class="image">
          <img
            src="./images/rsz_1photo-1414235077428-338989a2e8c0.jpg"
            alt=""
          />
        </div>
        <h3>Beef 25$</h3>
        <button>Order</button>
    </div>

    <div class="bigbox two">
      <div class="image">
        <img src="./images/rsz_photo-1466978913421-dad2ebd01d17.jpg" alt="" />
      </div>
      <h3>Pork 30$</h3>
      <button>Order</button>
    </div>

    <div class="bigbox three">
      <div class="image">
        <img src="./images/rsz_photo-1498654896293-37aacf113fd9.jpg" alt="" />
      </div>

      <h3>Fish 15$</h3>
      <button>Order</button>
    </div>

    <div class="bigbox four">
      <div class="image">
        <img src="./images/rsz_photo-1502301103665-0b95cc738daf.jpg" alt="" />
      </div>
      <h3>Chicken 10$</h3>
      <button>Order</button>
    </div>
  </body>
</html>

<styles>/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}
body {
  line-height: 1;
}
ol,
ul {
  list-style: none;
}
blockquote,
q {
  quotes: none;
}
blockquote:before,
blockquote:after,
q:before,
q:after {
  content: "";
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}

html {
  box-sizing: border-box;
  font-family: "Open Sans", sans-serif;
}

/* MY CSS */
body {
  min-height: 150vh;
}

/* Headings 1,2,3 */
h1 {
  color: rgb(0, 0, 0);
  font-size: 10vh;
  font-weight: 700;
  text-align: center;
  padding: 15vh 0;
  text-transform: uppercase;
  letter-spacing: 5px;
  background: linear-gradient(
    90deg,
    rgba(59, 5, 5, 1) 0%,
    rgba(255, 0, 0, 0.61) 53%,
    rgba(59, 5, 5, 1) 100%
  );
}

h2 {
  font-size: 7vh;
  font-weight: 400;
  text-align: center;
  background: linear-gradient(
    90deg,
    rgba(59, 5, 5, 1) 0%,
    rgba(255, 0, 0, 0.61) 53%,
    rgba(59, 5, 5, 1) 100%
  );
  padding: 15px 0;
  border-bottom: 2px solid rgba(0, 0, 0, 0.521);
}

h3 {
  font-size: 25px;
  margin-top: 15px;
  border-bottom: 2px solid rgba(139, 0, 0, 0.493);
  letter-spacing: 2px;
}

/* Navbar */

nav {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  background-color: black;
  color: white;
  height: 10vh;
}

nav ul {
  display: flex;
  align-content: space-around;
  padding: 10px;
}

nav ul li {
  padding: 0 12vw;
  font-size: 3vh;
  font-family: monospace;
  letter-spacing: 1px;
  border-right: 2px solid rgb(255, 0, 0);
}

#contact {
  border: none;
}

a {
  text-decoration: none;
  color: white;
}

a:hover,
a:active {
  color: red;
  letter-spacing: 3px;
  transition: 200ms;
}

/* Big container with menus */

.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  align-content: space-around;
  padding: 20px;
  background-image: url(./images/terasacrop2.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

.bigbox {
  border: 5px solid rgba(139, 0, 0, 0.87);
  margin: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
  flex-wrap: wrap;
  background-color: white;
  border-radius: 4px 4px 10px 10px;
}

/* Buttons inside menus */

button {
  margin: 35px 0;
  width: 30%;
  height: 5vh;
  border: none;
  background-color: rgba(139, 0, 0, 0.856);
  color: white;
  font-size: 17px;
  border-radius: 5px;
}

button:hover,
button:active {
  background-color: rgb(179, 7, 7);
  transition: 200ms;
  cursor: pointer;
  letter-spacing: 2px;
}

@media (max-width: 871px) {
  nav ul {
    width: 100%;
    background-color: rgb(0, 0, 0);
    display: flex;
    flex-direction: column;
    align-items: center;
    align-content: space-around;
    margin-top: 40px;
  }

  nav ul li {
    border: none;
    padding: 5px 0;
  }

  h1 {
    padding-top: 100px;
  }
}
</styles>
