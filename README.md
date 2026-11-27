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
