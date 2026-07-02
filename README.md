<svg width="470" height="120" viewBox="0 0 470 120" xmlns="http://www.w3.org/2000/svg">
  <style>
    .on {
      animation: glow 1.6s ease-in-out infinite alternate;
    }

    @keyframes glow {
      from { fill: #238636; opacity: 0.75; }
      to { fill: #39d353; opacity: 1; }
    }
  </style>

  <rect width="100%" height="100%" fill="#0d1117"/>

  <script>
    const letters = {
      D: [
        "11110",
        "10001",
        "10001",
        "10001",
        "10001",
        "10001",
        "11110"
      ],
      E: [
        "11111",
        "10000",
        "10000",
        "11110",
        "10000",
        "10000",
        "11111"
      ],
      P: [
        "11110",
        "10001",
        "10001",
        "11110",
        "10000",
        "10000",
        "10000"
      ],
      A: [
        "01110",
        "10001",
        "10001",
        "11111",
        "10001",
        "10001",
        "10001"
      ],
      K: [
        "10001",
        "10010",
        "10100",
        "11000",
        "10100",
        "10010",
        "10001"
      ]
    };

    const name = "DEEPAK";
    const size = 10;
    const gap = 3;
    const letterGap = 13;
    const startX = 20;
    const startY = 20;

    const svg = document.currentScript.parentNode;
    let delay = 0;

    name.split("").forEach((letter, letterIndex) => {
      const pattern = letters[letter];
      const offsetX = startX + letterIndex * ((size + gap) * 5 + letterGap);

      pattern.forEach((row, y) => {
        row.split("").forEach((cell, x) => {
          const rect = document.createElementNS("http://www.w3.org/2000/svg", "rect");

          rect.setAttribute("x", offsetX + x * (size + gap));
          rect.setAttribute("y", startY + y * (size + gap));
          rect.setAttribute("width", size);
          rect.setAttribute("height", size);
          rect.setAttribute("rx", 2);
          rect.setAttribute("fill", cell === "1" ? "#39d353" : "#161b22");

          if (cell === "1") {
            rect.setAttribute("class", "on");
            rect.setAttribute("style", `animation-delay:${delay.toFixed(2)}s`);
            delay += 0.035;
          }

          svg.appendChild(rect);
        });
      });
    });
  </script>
</svg>


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/89bb59e7-0b43-4282-a805-b9bcac0b1a19" />

<h1 align="center">Hi there 👋, I'm Deepak Rajesh</h1>
<h3 align="center">Aspiring AI/ML Engineer | Public speaking & Startup Enthusiast</h3>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=Building+Machine+Learning+Systems;NLP+%7C+Computer+Vision+%7C+Forecasting;Turning+Data+Into+Decisions;B.Tech+CSE+%40+VIT+Chennai" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/deepak-rajesh/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:deepakrajesh500@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://instagram.com/deezxribhu" target="_blank"> 
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" /> 
  </a> 
  <a href="https://x.com/DeepakRajesh9" target="_blank"> 
    <img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" /> 
  </a>
</p>

<br>


