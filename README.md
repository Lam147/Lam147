## Leonardo Melo 👋

🎓 Graduado em Análise e Desenvolvimento de Sistemas
 
📚 Estudando sobre:

💻 Testes e Qualidade de Software (QA)

🤖 Inteligência Artificial e Engenharia de Prompt

🇺🇸 Inglês


---
---

### 🤖 Linguagens e Tecnologias


  <img
    align="left" 
    alt="MySQL"
    title="MySQL" 
    width="30px" 
    style="padding-right: 10px;"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original-wordmark.svg" />

<img 
    align="left" 
    alt="HTML5"
    title="HTML5" 
    width="30px" 
    style="padding-right: 10px;"  
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg"
/>
<img 
    align="left" 
    alt="CSS3" 
    title="CSS3"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg"
/>
<img 
    align="left" 
    alt="JavaScript" 
    title="JavaScript"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg"
/>
<img 
    align="left" 
    alt="Git" 
    title="Git"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg"
/>
  <img
    align="left" 
    alt="Nodejs" 
    title="Nodejs"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original-wordmark.svg"
/>  

  <img
    align="left" 
    alt="Cypressio" 
    title="Cypressio"
    width="30px" 
    style="padding-right: 10px;"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/cypressio/cypressio-original-wordmark.svg"
/>


<img 
    align="left" 
    alt="GitHub Stats" 
    height="200" 
    src="https://github-readme-stats.vercel.app/api/top-langs/?username=LAM147&theme=tokyonight&layout=compact&custom_title=Tecnologias&langs_count=9" 
/>
  
  </p>



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
          github_user_name: LAM147
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  
