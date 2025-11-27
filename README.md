# MagusCode 🧙‍♂️💻

MagusCode é um mini-jogo educativo desenvolvido para a EXPOFADESA, dentro do eixo **Fundamentos da Computação e Programação**, com identidade visual inspirada na temática de **Halloween**.  
O objetivo do projeto é estimular o interesse pela área de tecnologia e treinar **lógica de programação** por meio de um sistema de **quiz** integrado à exploração de cenário e combate a inimigos.

---

## Objetivos do projeto

- Integrar conceitos básicos de programação (variáveis, condições, contadores) à mecânica de um jogo digital.
- Proporcionar uma experiência interativa que desperte o interesse pela área de computação.
- Estimular o raciocínio lógico, a resolução de problemas e a tomada de decisão por meio de desafios progressivos.

---

##  Mecânicas principais

- O jogador controla um personagem em um mapa 2D, enfrentando inimigos.
- Cada inimigo derrotado incrementa o contador `kills`.
- Ao alcançar uma **coordenada especial** no mapa:
  - Se `kills < 30`: aparece um **popup** avisando que é necessário eliminar **30 ou mais inimigos**.
  - Se `kills >= 30`: o jogador é **teletransportado para a biblioteca**.
- Na biblioteca, ao chegar na coordenada do ancião, inicia-se um **quiz de lógica de programação**:
  - A cada resposta errada, o contador `errosQuiz` é incrementado.
  - Com **2 erros**, o jogador é redirecionado para `gameover.html` (calabouço) e um **novo jogo** é iniciado.
  - Se o jogador acertar **todas as perguntas antes de errar 2 vezes**, torna-se **imortal e muito poderoso**.
- Após concluir o quiz com sucesso, o jogador volta ao mapa:
  - Agora imortal, precisa eliminar **100 inimigos**.
  - Ao atingir `kills >= 100`, é redirecionado para `zerou.html`, marcando que **zerou o jogo**.
  - A partir daí, o sistema reinicia a fase, permitindo começar com um **novo jogador**.

---

## Tecnologias utilizadas

- **HTML5** – estrutura do jogo e das páginas (`index.html`, `gameover.html`, `zerou.html`).
- **CSS3** – estilização, identidade visual e ambientação temática de Halloween.
- **JavaScript** – lógica do jogo, movimentação, colisões, contadores, quiz e redirecionamentos.

---

## Instalação e execução

1. Baixe ou clone este repositório:
   ```bash
   git clone https://github.com/SEU_USUARIO/maguscode.git
