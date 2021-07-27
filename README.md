<h2 align="center">Hey! Today I created bouncing text in pure HTML and CSS.</h2>
<div align="center"> 
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=HTML5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
<img src="https://img.shields.io/github/languages/code-size/Medvedoc/jumping-text?style=for-the-badge">
<img src="https://img.shields.io/tokei/lines/github/medvedoc/jumping-text?style=for-the-badge">
</div>
<div align="center">
<img src="https://img.shields.io/github/last-commit/medvedoc/jumping-text?style=for-the-badge">
<img src="https://img.shields.io/github/contributors/medvedoc/jumping-text?style=for-the-badge">
<img src="https://img.shields.io/github/license/medvedoc/jumping-text?style=for-the-badge">
<!--<img src="https://img.shields.io/github/commit-activity/m/mevedoc/jumping-text?style=for-the-badge">
<img src="https://img.shields.io/github/downloads/medvedoc/jumping-text/total?style=for-the-badge">-->
</div>
<h3 align="center">All animation is based on @keyframes.</h3>
<div align="center"><a href="https://cdn.buymeacoffee.com/uploads/project_updates/2021/07/efdf87aad26d7363cb9c224f008696ce.gif"><img src="https://cdn.buymeacoffee.com/uploads/project_updates/2021/07/efdf87aad26d7363cb9c224f008696ce.gif" /></a></div>
<h3 align="center">Demonstration: <a href="https://codepen.io/Medvedoc/full/yLbpePv">codepen</a></h3>
<h3 align="center">Download: <a href="https://github.com/Medvedoc/jumping-text/archive/refs/heads/main.zip">github</a></h3>

<h2>HTML code</h2>

```html
<div id="wrapper">
    <div id="container">
        <h1>Simple Text</h1>
    </div>
</div>
```

<h2>CSS code</h2>

```css
*, :before, :after {
    box-sizing: border-box;
}
body {
    background-color: #fff;
    font: 16px/1.25 'Titan one', sans-serif;
    text-align: center;
}
#wrapper {
    margin: 0 auto;
}
#container {
    display: flex;
    flex-direction: column;
    float: left;
    justify-content: center;
    min-height: 100vh;
    padding: 1em;
    width: 100%;
}
h1 {
    animation: text-shadow 2s ease-in-out infinite;
    font-size: 5em;
    font-weight: 900;
    line-height: 1;
    color: #ec4f43;
}
@keyframes text-shadow {
    0% {
        transform: translateY(0);
        text-shadow:
            0 0 0 #fe7968,
            0 0 0 #fe948d,
            0 0 0 #ffbdb3,
            0 0 0 #ffe0db;
    }
    20% {
        transform: translateY(-0.2em);
        text-shadow:
            0 0.125em 0 #fe7968,
            0 0.25em 0 #fe948d,
            0 -0.125em 0 #ffbdb3,
            0 -0.25em 0 #ffe0db;
    }
    40% {
        transform: translateY(0.1em);
        text-shadow:
            0 -0.0625em 0 #fe7968,
            0 -0.125em 0 #fe948d,
            0 0.0625em 0 #ffbdb3,
            0 0.125em 0 #ffe0db;
    }
    60% {
        transform: translateY(-0.1em);
        text-shadow:
            0 0.03125em 0 #fe7968,
            0 0.0625em 0 #fe948d,
            0 -0.03125em 0 #ffbdb3,
            0 -0.0625em 0 #ffe0db;
    }
    80% {
        transform: translateY(0);
        text-shadow:
            0 0 0 #fe7968,
            0 0 0 #fe948d,
            0 0 0 #ffbdb3,
            0 0 0 #ffe0db;
    }
}
```
