# 🐍 Jogo da Cobrinha

Um jogo clássico de cobrinha desenvolvido com **HTML5, CSS3 e JavaScript puro**, executado diretamente no navegador, sem necessidade de instalar programas, bibliotecas ou frameworks externos.

O objetivo é controlar a cobrinha, coletar alimentos, acumular pontos e tentar superar o próprio recorde sem bater nas paredes ou no próprio corpo.

## 📋 Sobre o projeto

O projeto recria a experiência do tradicional jogo da cobrinha com uma interface moderna, controles intuitivos e recursos que tornam a experiência mais agradável em computadores, celulares e tablets.

### ✨ Funcionalidades

- 🐍 Movimentação da cobrinha em quatro direções.
- 🍎 Alimentos gerados aleatoriamente no tabuleiro.
- 📈 Sistema de pontuação: cada alimento vale 10 pontos.
- 🏆 Recorde salvo no navegador.
- ⚡ Aumento gradual da velocidade conforme a pontuação cresce.
- ⏸️ Opção para pausar e retomar a partida.
- 🔄 Botão para reiniciar o jogo.
- 💥 Detecção de colisões com as paredes e com o próprio corpo.
- 🎉 Mensagem de vitória ao preencher todo o tabuleiro.
- 📱 Controles direcionais para dispositivos com tela sensível ao toque.
- 🎨 Interface responsiva com tema escuro e elementos visuais modernos.
- ♿ Recursos de acessibilidade, como rótulos descritivos e indicação visual de foco nos botões.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar o conteúdo e os elementos da interface do jogo.

Principais recursos:
- Organização semântica com elementos como `main`, `header` e `section`.
- Botões para iniciar, pausar, retomar e reiniciar a partida.
- Elemento `canvas` para desenhar o tabuleiro, a cobrinha e os alimentos.
- Atributos de acessibilidade para auxiliar na identificação dos elementos.

### 🎨 CSS3

Responsável pela aparência visual e pela adaptação da interface a diferentes tamanhos de tela.

Principais recursos:
- Flexbox e CSS Grid para organizar os elementos.
- Variáveis CSS para centralizar cores e facilitar a personalização.
- Media queries para adaptar o layout a telas menores.
- Bordas arredondadas, sombras, gradientes e efeitos visuais.
- Estados visuais para interação com os botões.
- Suporte à preferência do usuário por redução de animações.

### ⚙️ JavaScript (Vanilla JavaScript)

Responsável por toda a lógica e interatividade do jogo, sem dependência de bibliotecas externas.

Principais recursos:
- Controle da movimentação e da direção da cobrinha.
- Atualização da pontuação e do recorde.
- Geração aleatória de alimentos em posições livres.
- Verificação de colisões e condições de vitória.
- Controle dos estados da partida: pronto, jogando, pausado, fim de jogo e vitória.
- Gerenciamento do tempo de movimentação com `setTimeout`.
- Manipulação dos elementos HTML por meio do DOM.
- Captura de eventos de teclado e cliques nos controles.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada pelo JavaScript para desenhar os elementos gráficos do jogo.

O tabuleiro possui uma área de desenho de 400 × 400 pixels, dividida em uma grade de 20 × 20 células.

A cobrinha é representada por segmentos verdes, enquanto o alimento aparece como um círculo vermelho. A cabeça da cobrinha possui uma tonalidade mais clara e olhos orientados conforme a direção do movimento.

### 💾 LocalStorage

Utilizado para armazenar o recorde no próprio navegador, permitindo que a melhor pontuação seja recuperada em visitas futuras no mesmo navegador e perfil.

Caso o armazenamento esteja indisponível, o jogo continua funcionando, embora o recorde possa não ser preservado após o encerramento da sessão.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo:

```text
jogo-da-cobrinha/
└── index.html
```

O arquivo `index.html` contém:

- **HTML:** estrutura da página e dos controles.
- **CSS:** estilos e responsividade.
- **JavaScript:** regras, movimentação, pontuação e interações.

Essa organização simplifica a execução, o compartilhamento e o estudo do código.

## ▶️ Como executar o projeto

Não é necessário instalar dependências, configurar um servidor ou utilizar ferramentas adicionais.

1. 📥 Baixe ou copie o arquivo `index.html` para o seu computador.
2. 📂 Localize o arquivo na pasta em que foi salvo.
3. 🖱️ Dê dois cliques no arquivo ou abra-o em um navegador moderno.
4. 🎮 Clique no botão **Começar** ou utilize os controles direcionais para iniciar a partida.
5. 🚀 Divirta-se tentando alcançar a maior pontuação possível!

**Requisito:** um navegador moderno, como Google Chrome, Microsoft Edge, Mozilla Firefox ou Safari.

## 🎮 Modo de jogar

### 1. Iniciar a partida

Clique no botão **Começar** para iniciar uma nova partida. Também é possível utilizar as teclas direcionais ou as teclas WASD para iniciar e movimentar a cobrinha.

### 2. Controlar a cobrinha

Utilize os seguintes comandos:

| Ação | Teclado |
|---|---|
| ⬆️ Mover para cima | Seta para cima ou `W` |
| ⬇️ Mover para baixo | Seta para baixo ou `S` |
| ⬅️ Mover para a esquerda | Seta para a esquerda ou `A` |
| ➡️ Mover para a direita | Seta para a direita ou `D` |
| ⏸️ Pausar ou retomar | Barra de espaço |

Em celulares e tablets, utilize os botões direcionais exibidos abaixo do tabuleiro.

**Dica:** a cobrinha não pode inverter diretamente o sentido do movimento. Por exemplo, se estiver indo para a direita, não será possível fazê-la virar imediatamente para a esquerda.

### 3. 🍎 Coletar alimentos

O alimento aparece em uma posição livre do tabuleiro.

Sempre que a cobrinha comer um alimento:

- A pontuação aumenta em 10 pontos.
- O corpo da cobrinha cresce.
- A velocidade aumenta gradualmente.
- O recorde é atualizado quando a pontuação atual supera a melhor marca registrada.

### 4. ⚠️ Evitar colisões

A partida termina quando a cabeça da cobrinha:

- Atinge uma das paredes do tabuleiro.
- Colide com o próprio corpo.

Planeje as curvas com antecedência para evitar acidentes, especialmente quando a cobrinha estiver maior e mais rápida.

### 5. ⏸️ Pausar e retomar

Clique em **Pausar** para interromper temporariamente a partida. Para continuar, clique em **Retomar** ou pressione a barra de espaço.

O jogo também pausa automaticamente quando a aba do navegador perde a visibilidade durante uma partida.

### 6. 🔄 Reiniciar a partida

Clique em **Reiniciar** para começar uma nova partida imediatamente, zerando a pontuação atual e restaurando a velocidade inicial.

O recorde salvo é mantido.

### 7. 🏆 Vencer o jogo

A vitória acontece quando a cobrinha ocupa todas as células do tabuleiro, sem deixar posições livres para a geração de novos alimentos.

Ao vencer, uma mensagem especial é exibida na tela.

## 📊 Regras e características técnicas

| Característica | Descrição |
|---|---|
| 📐 Tabuleiro | 20 × 20 células |
| 🎯 Pontuação por alimento | 10 pontos |
| ⏱️ Intervalo inicial | 165 milissegundos por movimento |
| ⚡ Intervalo mínimo | 72 milissegundos por movimento |
| 📉 Redução do intervalo | 4 milissegundos por alimento, até o limite mínimo |
| 🍎 Geração de alimentos | Aleatória, em células livres |
| 💾 Recorde | Armazenado com `localStorage` |
| 🧩 Arquivos necessários | Apenas `index.html` |
| 🌐 Execução | Diretamente no navegador |

## 🎯 Objetivos educacionais

Este projeto também pode ser utilizado como exercício de aprendizado para quem está começando no desenvolvimento web.

Com ele, é possível estudar:

- 📄 Estruturação de páginas com HTML.
- 🎨 Estilização e responsividade com CSS.
- 🧠 Variáveis, constantes, funções e estruturas condicionais em JavaScript.
- 🔁 Laços de repetição e manipulação de arrays.
- 🎮 Desenvolvimento de lógica para jogos.
- 🖌️ Desenho de gráficos com Canvas API.
- ⌨️ Tratamento de eventos de teclado e cliques.
- 💾 Persistência de dados no navegador.
- 🛡️ Verificação de colisões e controle de estados.
- 📱 Criação de interfaces adaptáveis a diferentes dispositivos.

## 🚀 Possíveis melhorias futuras

O projeto pode ser ampliado com novas funcionalidades, como:

- 🔊 Efeitos sonoros para movimentos, alimentos e colisões.
- 🎵 Música de fundo com opção de ativar ou desativar.
- 🎨 Temas visuais alternativos para a cobrinha e o tabuleiro.
- 🥇 Histórico das melhores pontuações.
- 🎚️ Seleção de níveis de dificuldade.
- ⏳ Cronômetro e estatísticas da partida.
- 🌐 Ranking online de jogadores.
- 🕹️ Novos modos de jogo e obstáculos especiais.

## 📜 Licença

Este projeto pode ser utilizado como material de estudo e prática de desenvolvimento web. Caso seja distribuído publicamente, recomenda-se definir uma licença explícita para estabelecer as condições de uso, modificação e redistribuição.

---

**Desenvolvido com 💚 HTML5, CSS3 e JavaScript puro.**

🐍 **Coma, cresça e tente bater seu recorde!**
