## 💻 Evellyn Pedroso  
**Desenvolvedora de Software**  

Me chamo Evellyn, tenho 20 anos e sou natural de São Paulo.  
Sou estudante de Engenharia de Software na Universidade Católica de Salvador.  
Além de desenvolvedora, também sou professora de inglês e espanhol.  


<p align="center">
  <table>
    <tr>
      <td>
        <img height="180em" src="https://github-readme-stats.vercel.app/api?username=evellynpedroso&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true"/>
      </td>
      <td>
        <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=evellynpedroso&layout=compact&langs_count=7&theme=tokyonight"/>
      </td>
    </tr>
  </table>
</p>
 

<div style="display: inline_block"><br>
  <img align="center" alt="Rafa-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="Rafa-Ts" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-plain.svg">
  <img align="center" alt="Rafa-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="Rafa-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
    <img align="center" alt="Rafa-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg">
</div>
</div>

---
## 🗺 Conecte-se comigo  

[![Linkedin Badge](https://img.shields.io/badge/-Evellyn%20Miranda-blue?style=for-the-badge&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/evellyn-miranda-3ab790224)](https://www.linkedin.com/in/evellyn-miranda-3ab790224)  
[![Gmail Badge](https://img.shields.io/badge/-evellynpstudy@gmail.com-c14438?style=for-the-badge&logo=Gmail&logoColor=white&link=mailto:evellynpstudy@gmail.com)](mailto:evellynpstudy@gmail.com)

---
name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  

