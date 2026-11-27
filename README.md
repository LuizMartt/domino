# Dominó (título provisório)

Dominó de verdade contra bots, com níveis, coringas, loja e desafios. É um jogo de navegador num arquivo só (`index.html`), sem instalação.

## Como jogar

Abra o `index.html` no navegador, no computador ou no celular.

- **1×1:** você contra um bot. Cada um recebe 7 pedras e sobram 14 no banco para comprar.
- **1×3:** quatro na mesa, cada um por si. As 28 pedras são distribuídas.
- **Batida:** quem bate soma os pontos que sobraram na mão dos outros.
  - **Bucha** (bater com uma dupla): +5.
  - **Lá e lô** (pedra que serve nas duas pontas): +10.
  - **Cruzada** (dupla que serve nas duas pontas): +20.
- **Mesa trancada:** ninguém consegue jogar e o banco acabou. Vence quem tiver menos pontos na mão.
- **Mãos (vidas):** você tem 3 mãos por nível. Cada mão que um bot vence gasta uma. Se acabarem antes de você chegar à meta, a run recomeça do início.
- **Níveis:** são 8, e os níveis 3, 6 e 8 são chefes. Os bots ficam mais espertos a cada 3 níveis.
- **Coringas:** os passivos ficam sempre ligados. Os ativos têm 1 uso por mão.

## Jogar online (GitHub Pages)

Em **Settings → Pages**, escolha *Deploy from a branch*, depois a branch `main` e a pasta `/ (root)`. Em um ou dois minutos o jogo fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Estrutura

| Arquivo | O que é |
|---|---|
| `index.html` | O jogo inteiro: HTML, CSS e JavaScript |

## Status

Protótipo em desenvolvimento (v0.5).

## Novidades desta versão

- Tela inicial nova, com redemoinho animado, logo e dicas.
- Uma música 8-bit para cada nível, cada vez mais rápida e sombria, e um tema próprio na tela inicial.
- 3 mãos (vidas) por nível. Se acabarem, a run volta ao início.
- As pedras voam até a mesa ao serem jogadas, tanto as suas quanto as dos bots.
- Bots com as pedras em pé num suporte de madeira, ao redor da mesa.
- Configurações novas: música, velocidade dos bots, ordem da mão, cor do tabuleiro, costas das pedras, tela cheia e estatísticas.
- Explicação de como os bots jogam em cada dificuldade.
- Loja com popup ao passar o mouse ou tocar no coringa.
- Painel compacto no celular e fonte mais legível.
