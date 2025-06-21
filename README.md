# 💫 Sobre mim:
Meu nome é Abel, tenho 18 anos e moro em Itaquaquecetuba. Quando eu comecei o curso do Proa eu possuía apenas o básico em HTML e CSS, junto a uma rasa introdução em C# e Arduino. Fiz curso técnico junto ao Ensino Médio na Etec de Itaquaquecetuba em Desenvolvimento de Sistemas (DS), e no Senai de Mogi eu fiz um curso de Fundamentos do Java, onde adquiri o certificado da Oracle nesta linguagem. Não curso no momento nenhuma faculdade, mas intento fazer Engenharia de Computação ou Sistemas de Informação. Pretendo me aprimorar nas linguagens C#, e dominar o que não pude em Java e Javascript para as utilizar no mercado de trabalho. Viso atuar na área de FrontEnd, BackEnd ou Full Stack.


## 🌐 Redes Sociais:
[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/https://discord.gg/y4dRvnJQ) [![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/https://www.instagram.com/abelgarcia83/) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/https://www.linkedin.com/in/abelgarcia7/) [![email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:abel89275@gmail.com) 

# 💻 Ferramentas Dev - Tech Stack:
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=plastic&logo=csharp&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=plastic&logo=javascript&logoColor=%23F7DF1E) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=plastic&logo=css3&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=plastic&logo=html5&logoColor=white) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=plastic&logo=.net&logoColor=white) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=plastic&logo=react&logoColor=%2361DAFB) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=plastic&logo=mysql&logoColor=white) ![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=plastic&logo=microsoft%20sql%20server&logoColor=white) ![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=plastic&logo=figma&logoColor=white) ![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=plastic&logo=Canva&logoColor=white) ![Gimp](https://img.shields.io/badge/Gimp-657D8B?style=plastic&logo=gimp&logoColor=FFFFFF) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=plastic&logo=github&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=plastic&logo=git&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=Abel2007u&theme=dark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://nirzak-streak-stats.vercel.app/?user=Abel2007u&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=Abel2007u&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=Abel2007u&theme=radical&no-frame=false&no-bg=true&margin-w=4)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

### 🔝 Top Contributed Repo
![](https://github-contributor-stats.vercel.app/api?username=Abel2007u&limit=5&theme=dark&combine_all_yearly_contributions=true)

---
[![](https://visitcount.itsvg.in/api?id=Abel2007u&icon=0&color=0)](https://visitcount.itsvg.in)

---
name: Generate snake animation

on:
  schedule:
    # Executa a cada 12 horas
    - cron: "0 */12 * * *"
  workflow_dispatch:
  push:
    branches:
      - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: Generate snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: Abel2007u
          outputs: dist/snake.svg?palette=github-dark

      - name: Push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}


<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
