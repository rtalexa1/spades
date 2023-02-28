<template>
  <div class="container">
    <RouterView />
  </div>
  <footer>
    <span>Copyright 2023 RT Alexander</span> |
      <span>Contact: rtalexa1@gmail.com</span>
      <p v-if="$route.path === '/'">
        Photo by 
        <a 
          href="https://unsplash.com/@adityachinchure?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText"
          >Aditya Chinchure</a
          > 
        on 
        <a 
          href="https://unsplash.com/photos/DT5WpTYvo1c?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText"
          >Unsplash</a
        >
      </p>
  </footer>
</template>

<style lang="scss">
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}

/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}

body {
  overflow: scroll;
  min-height: 100%;
	background-image: url("./assets/spades-background-photo.jpg"); 
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top;
  font-size: medium;
  line-height: 1.5;
  font-family: 'Fugaz One', cursive;
}

ol, ul {
	list-style: none;
}

blockquote, q {
	quotes: none;
}

blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}

table {
	border-collapse: collapse;
	border-spacing: 0;
}

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}

footer {
  width: 100%;
  padding: 2px 10px;
  background: #f9f9f9;
  font-size: x-small;
  text-align: center;
}
</style>
