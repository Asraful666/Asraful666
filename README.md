<!-- ===================== HEADER BANNER ===================== -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:667eea,100:764ba2&height=220&section=header&text=Md%20Asraful%20Islam&fontSize=45&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=CSE%20Student%20%7C%20Aspiring%20Full-Stack%20Developer&descAlignY=55&descSize=18" width="100%"/>

</div>


# Hi 👋, I'm Md Asraful Islam

### 💻 CSE Student | Aspiring Full-Stack Developer

I'm a passionate Computer Science & Engineering student who enjoys building modern and responsive web applications. I'm currently focusing on improving my skills in **JavaScript, React, Tailwind CSS, and Node.js** while working on real-world projects.

I enjoy learning new technologies, solving programming problems, and turning ideas into useful web applications.

---

## 👨‍💻 About Me

- 🎓 Computer Science & Engineering Student
- 💻 Interested in Web Development & Full-Stack Development
- 🌱 Currently learning JavaScript, React & Backend Development
- 🚀 Building projects to improve my development skills
- 📚 Interested in Programming, Web Development & Technology
- ⚡ Always trying to learn something new

---

## 🛠️ Tech Stack

### 🌐 Frontend

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)

![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=white)

### ⚙️ Backend

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)

![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

### 🔧 Tools

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

---

## 🚀 Featured Projects

### 🍽️ Restaurant Menu

A responsive restaurant menu project built with HTML and CSS.

### 🎤 DevConf 2026

A conference landing page built with modern HTML, CSS and responsive design.

### 👤 Personal Profile Card

A clean personal profile card created using modern CSS layout techniques.

### 📈 Stock Market Simulator

A web-based stock market simulator project using HTML, CSS and JavaScript.

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Asraful666&show_icons=true&theme=default&hide_border=true" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Asraful666&layout=compact&theme=default&hide_border=true" />

</div>

---

## 🌐 Connect With Me

<p align="left">

<a href="https://github.com/Asraful666">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

</p>

---

## 📈 Profile Views

<img src="https://komarev.com/ghpvc/?username=Asraful666&style=for-the-badge" />

---

### 💡 Keep learning, keep building, keep improving.

⭐ Thanks for visiting my profile!



## 📊 GITHUB STATISTICS & ANALYSIS

### 🐍 GitHub Contributions

<div align="center">

<img src="https://raw.githubusercontent.com/Asraful666/Asraful666/output/grid.svg" alt="GitHub Contribution Snake" width="100%">

</div>

---

### 📊 GitHub Statistics

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Asraful666&theme=swift&hide_border=true&include_all_commits=false&count_private=false" height="180">

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Asraful666&theme=swift&hide_border=true&include_all_commits=false&count_private=false&layout=compact" height="180">

</div>

---

### 🔥 Repository Stats & Streak

<div align="center">

<img src="https://github-contributor-stats.vercel.app/api?username=Asraful666&limit=5&theme=swift&combine_all_yearly_contributions=true&hide_border=true" height="180">

<img src="https://streak-stats.demolab.com/?user=Asraful666&theme=swift&hide_border=true" height="180">

</div>

---

## 💡 RANDOM DEV QUOTE

<div align="center">

<img src="https://quotes-github-readme.vercel.app/api?type=vertical&theme=light" alt="Random Dev Quote">

</div>

---

<div align="center">

<img src="https://komarev.com/ghpvc/?username=Asraful666&label=Profile%20Views&color=0e75b6&style=flat" alt="Profile Views">

</div>
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
  push:
    branches:
      - main

jobs:
  generate:
    permissions:
      contents: write

    runs-on: ubuntu-latest

    steps:
      - name: Generate Snake
        uses: Platane/snk@v3
        with:
          github_user_name: Asraful666
          outputs: |
            dist/grid.svg
            dist/grid-dark.svg?palette=github-dark

      - name: Deploy Snake
        uses: crazy-max/ghaction-github-pages@v4
        with:
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          BUILD_DIR: dist
