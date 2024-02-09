# **READ-ME / LEIA-ME**

```bash
#!/bin/bash

msg_pt_BR_UTF_8="Olà Mundo! Eu sou o Nicolau"
msg_en_US_UTF_8="Hello World! I'm the Nicolau"
variaveis=("msg_pt_BR_UTF_8" "msg_en_US_UTF_8")
idioma_atual=$LANG

for variavel in "${variaveis[@]}"; do
    if [[ $idioma_atual == *"pt_BR"* ]] && [[ $variavel == "msg_pt_BR_UTF_8" ]]; then
        mensagem=${!variavel}
        printf "%s\n" "Mensagem em Português (Brasil): $mensagem"
    elif [[ $idioma_atual == *"en_US"* ]] && [[ $variavel == "msg_en_US_UTF_8" ]]; then
        mensagem=${!variavel}
        printf "%s\n" "Message in English (United States): $mensagem"
    fi
done
```

| numero | destino|
|---|---|
| 1 | [ Anotações ](./Notes/pt_BR.UTF-8.md)

---

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=kolyasik-inc&show_icons=true&theme=transparent&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)
 
<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg"
  />
  <source
    media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
  />
  <img
    alt="github contribution grid snake animation"
    src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
  />
</picture>

<!--
<div>
  <a href="https://www.youtube.com/channel/UCEzUJF1OH0n6dnPIXe5hpCg" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" target="_blank"></a>
  <a href="https://instagram.com/nicolaslopes.inc" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
 	<a href="https://www.twitch.tv/oryvny" target="_blank"><img src="https://img.shields.io/badge/Twitch-9146FF?style=for-the-badge&logo=twitch&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  </div> 
 -->
