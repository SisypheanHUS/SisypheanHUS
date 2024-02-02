### Hi there 👋

🤔 I'am studying at Ha Noi University of Science (HUS)
- 🌱 I’m currently learning Java and Japanese,also trying to be Java Developer in Japan
<!--
**SisypheanHUS/SisypheanHUS** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->




![SisypheanHUS's Streak](https://github-readme-streak-stats.herokuapp.com/?user=SisypheanHUS&theme=tokyonight&hide_border=true)



![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=sisypheanhus&theme=tokyonight)

name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
  workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
