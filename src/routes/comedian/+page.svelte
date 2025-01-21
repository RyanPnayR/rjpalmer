<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  padding: 0;
  background-color: #34495e;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  overflow: hidden;
}

.spin-container {
  width: 500px;
  height: 500px;
  background-color: #ccc;
  border-radius: 50%;
  border: 15px solid #dde;
  position: absolute;
  overflow: hidden;
  transition: 5s;
}

.spin-container div {
  height: 50%;
  width: 50%;
  position: absolute;
  transform: rotate(calc(90deg * var(--i)));
  display: flex;
  align-items: center;
  justify-content: center;
  user-select: none;
  transform-origin: bottom right;
}

.spin-container .one {
  background-color: #3f51b5;
  clip-path: polygon(50% 0%, 100% 0, 100% 100%, 0 100%, 0 0);
}
.spin-container .two {
  background-color: #ff9800;
}
.spin-container .three {
  background-color: #e91e63;
}

.spin-container .four {
  background-color: green;
}

.arrow {
  position: absolute;
  color: #fff;
  top: -75%;
  left: 30%;
  rotate: 180deg;
}

.arrow::before {
  content: "\1F817";
  font-size: 50px;
}

#spin {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 10;
  background-color: #e2e2e2;
  text-transform: uppercase;
  border: 8px solid #fff;
  font-weight: bold;
  font-size: 20px;
  color: #a2a2a2;
  width: 80px;
  height: 80px;
  font-family: sans-serif;
  border-radius: 50%;
  cursor: pointer;
  outline: none;
  letter-spacing: 1px;
}

.spin-container div span {
  rotate: -45deg;
  color: white;
  font-weight: 900;
}
</style>

<script lang="js">
  import { onMount } from 'svelte';
  import * as Card from "$lib/components/ui/card";

  let container;
  let btn;
  let number;

  onMount(() => {
    container = document.querySelector(".spin-container");
    btn = document.getElementById("spin");
    number = Math.ceil(Math.random() * 10000);

    btn.onclick = function () {
      container.style.transform = "rotate(" + number + "deg)";
      number += Math.ceil(Math.random() * 10000);
      container.addEventListener("transitionend", SelectWinningAnswer, false);
    };
  });

  function SelectWinningAnswer() {
    const targetElement = document.querySelector(".arrow");

    const otherElements = document.querySelectorAll(".option");
    let topElement = otherElements[0];
    for (const otherElement of otherElements) {
      const otherRect = otherElement.getBoundingClientRect();
      topElement =
        topElement.getBoundingClientRect().top < otherRect.top
          ? topElement
          : otherElement;
    }
    console.log(topElement.textContent);
  }
</script>

<div class="grid place-items-center grid-cols-1 gap-1 h-screen">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Spin Wheel</title>
</head>

<body>
  <button id="spin"> <span class="arrow"></span>Spin</button>

  <div class="spin-container">
    <div class="option one" style="--i:1"><span>Speak No Evil</span></div>
    <div class="option two" style="--i:2"><span>Hear No Evil</span></div>
    <div class="option three" style="--i:3"><span>See No Evil</span></div>
    <div class="option four" style="--i:4"><span>Host Pick</span></div>
  </div>
</body>
</div>
