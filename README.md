## STEP 1 — GitHub Action Setup (metrics SVG generate karne ke liye)
## File path: .github/workflows/metrics.yml
## Apne repo mein yeh file banao

name: GitHub Metrics
on:
  schedule:
    - cron: "0 0 * * *"   # Daily auto-update
  workflow_dispatch:       # Manual trigger bhi kar sakte ho

jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          token: ${{ secrets.METRICS_TOKEN }}
          user: SunnyAgrwl05
          template: classic
          base: header, activity, community, repositories, metadata
          config_timezone: Asia/Kolkata

          # ── LANGUAGES ──
          plugin_languages: yes
          plugin_languages_analysis_timeout: 15
          plugin_languages_categories: markup, programming
          plugin_languages_colors: github
          plugin_languages_limit: 8
          plugin_languages_recent_categories: markup, programming
          plugin_languages_recent_days: 14
          plugin_languages_recent_load: 300
          plugin_languages_sections: most-used
          plugin_languages_threshold: 0%

          # ── LEETCODE ──
          plugin_leetcode: yes
          plugin_leetcode_limit_recent: 2
          plugin_leetcode_limit_skills: 10
          plugin_leetcode_sections: solved, skills, recent
          plugin_leetcode_user: Sunnyajit

          # ── TOPICS ──
          plugin_topics: yes
          plugin_topics_limit: 15
          plugin_topics_mode: starred
          plugin_topics_sort: stars

          # ── ACHIEVEMENTS ──
          plugin_achievements: yes
          plugin_achievements_display: detailed
          plugin_achievements_secrets: yes
          plugin_achievements_threshold: C

          # ── ACTIVITY ──
          plugin_activity: yes
          plugin_activity_days: 14
          plugin_activity_filter: all
          plugin_activity_limit: 5
          plugin_activity_load: 300
          plugin_activity_visibility: all

          # ── CONTRIBUTIONS CALENDAR ──
          plugin_calendar: yes
          plugin_calendar_limit: 1

          # ── WAKATIME (optional — agar use karte ho) ──
          # plugin_wakatime: yes
          # plugin_wakatime_token: ${{ secrets.WAKATIME_TOKEN }}
          # plugin_wakatime_limit: 5

---

## STEP 2 — README.md (metrics SVG use karne wala)
## Neeche wala code apne sunnyajit/sunnyajit README.md mein paste karo

<!-- HEADER -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=170&section=header&text=Sunny%20Kumar&fontSize=52&fontColor=fff&animation=twinkling&fontAlignY=36&desc=Full-Stack%20SDE%20%7C%20Open%20Source%20%7C%20Competitive%20Programmer&descAlignY=55&descSize=16" width="100%"/>
</div>

<!-- BADGES -->
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=SunnyAgrwl05&label=Profile+Views&color=0e75b6&style=flat-square"/>
  &nbsp;
  <a href="https://www.linkedin.com/in/sunny-kumar-a06484297/"><img src="https://img.shields.io/badge/LinkedIn-Open%20to%20Work-0077B5?style=flat-square&logo=linkedin&logoColor=white"/></a>
  &nbsp;
  <a href="mailto:sunnykumar98012085@gmail.com"><img src="https://img.shields.io/badge/Gmail-Hire%20Me-D14836?style=flat-square&logo=gmail&logoColor=white"/></a>
  &nbsp;
  <a href="YOUR_RESUME_LINK"><img src="https://img.shields.io/badge/Resume-Download-4CAF50?style=flat-square&logo=googledrive&logoColor=white"/></a>
</div>

<br/>

---

## 🌟 Open Source

<div align="center">

| Program | Role | Achievement |
|:---:|:---:|:---:|
| 🟠 **GSSoC** | Active Contributor | PRs Merged ✅ |
| 🎃 **Hacktoberfest** | Level 4 🏅 | Completed ✅ |

</div>

<div align="center">
  <img src="https://holopin.me/sunnyajit" width="82%" alt="Holopin Badges"/>
</div>

---

## 👨‍💻 About Me

```typescript
const sunny = {
  role   : "Full-Stack Software Engineer 🚀",
  college: "B.Tech — [YOUR COLLEGE]",
  stack  : ["C++", "Java", "JavaScript", "TypeScript", "Python"],
  openTo : "SDE Internship & Full-Time Roles 💼",
  solved : "441+ LeetCode | GSSoC | Hacktoberfest Lv4"
};
```
> 🔭 Building → **[YOUR PROJECT]** &nbsp;|&nbsp; 🌱 Learning → **System Design · Next.js · LLMs**

---

## 📊 GitHub Metrics (Auto-Updated Daily ✨)

<!-- After running the GitHub Action, these SVGs will appear automatically -->
<div align="center">
  <img src="github-metrics.svg" width="100%" alt="GitHub Metrics"/>
</div>

<!-- Fallback stats while metrics SVG generates -->
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=SunnyAgrwl05&theme=tokyonight&show_icons=true&hide_border=true&count_private=true" height="150"/>
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SunnyAgrwl05&theme=tokyonight&hide_border=true&layout=compact&langs_count=6" height="150"/>
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=SunnyAgrwl05&theme=tokyonight&hide_border=true" height="145"/>
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=SunnyAgrwl05&theme=tokyo-night&hide_border=true&area=true" width="92%"/>
</div>

---

## 🚀 Featured Projects

<table>
<tr>
<td width="50%">
<h3 align="center">📌 Project Name 1</h3>
<div align="center">
  <a href="YOUR_LIVE"><img src="https://via.placeholder.com/370x180/0d1117/00D9FF?text=▶+Live+Demo" width="92%"/></a><br/><br/>
  <a href="YOUR_REPO"><img src="https://img.shields.io/badge/Code-black?style=flat-square&logo=github"/></a>
  <a href="YOUR_LIVE"><img src="https://img.shields.io/badge/Live-00D9FF?style=flat-square&logo=vercel&logoColor=black"/></a><br/>
  <sub><b>React · Node.js · MongoDB · Docker</b></sub><br/>
  <sub>What it does + what problem it solves.</sub>
</div>
</td>
<td width="50%">
<h3 align="center">📌 Project Name 2</h3>
<div align="center">
  <a href="YOUR_LIVE"><img src="https://via.placeholder.com/370x180/0d1117/A78BFA?text=▶+Live+Demo" width="92%"/></a><br/><br/>
  <a href="YOUR_REPO"><img src="https://img.shields.io/badge/Code-black?style=flat-square&logo=github"/></a>
  <a href="YOUR_LIVE"><img src="https://img.shields.io/badge/Live-A78BFA?style=flat-square&logo=vercel&logoColor=black"/></a><br/>
  <sub><b>Python · FastAPI · PostgreSQL · GCP</b></sub><br/>
  <sub>What it does + what problem it solves.</sub>
</div>
</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JS](https://img.shields.io/badge/JS-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TS](https://img.shields.io/badge/TS-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=next.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=flat-square&logo=docker&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🏆 Competitive Programming

<div align="center">

| Platform | Handle | Stats | Link |
|:---:|:---:|:---:|:---:|
| 🟡 LeetCode | Sunnyajit | **441 solved** | [![](https://img.shields.io/badge/Visit-orange?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/u/Sunnyajit/) |
| 🟢 GFG | sunnykumarexcc | Active | [![](https://img.shields.io/badge/Visit-2F8D46?style=flat-square&logo=geeksforgeeks&logoColor=white)](https://www.geeksforgeeks.org/user/sunnykumarexcc/) |
| 🔵 Codeforces | sunajit | Rated | [![](https://img.shields.io/badge/Visit-1F8ACB?style=flat-square&logo=codeforces&logoColor=white)](https://codeforces.com/profile/sunajit) |
| 🔴 CodeChef | sunnykumar9801 | Active | [![](https://img.shields.io/badge/Visit-5B4638?style=flat-square&logo=codechef&logoColor=white)](https://www.codechef.com/users/sunnykumar9801) |

</div>

<div align="center">
  <img src="https://leetcard.jacoblin.cool/Sunnyajit?theme=dark&font=Fira%20Code&ext=heatmap&hide_border=true" width="44%"/>
  &nbsp;
  <img src="https://leetcard.jacoblin.cool/Sunnyajit?theme=dark&font=Fira%20Code&ext=contest&hide_border=true" width="44%"/>
</div>

---

## 🤝 Connect

<div align="center">
  <a href="https://www.linkedin.com/in/sunny-kumar-a06484297/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://x.com/SunnyTechLead"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white"/></a>
  <a href="https://www.youtube.com/@TechWithSunny90"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/></a>
  <a href="mailto:sunnykumar98012085@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>

<br/><br/>
<b>💼 Open to SDE Internship & Full-Time Roles!</b>
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&animation=twinkling" width="100%"/>
</div>
