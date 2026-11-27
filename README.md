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

## Online com amigos

Na tela inicial, toque em **Online**.

- **Criar sala:** escolha 1×1, 2×2 ou Todos (4 na mesa, cada um por si) e a meta de pontos. Você recebe um código de 5 letras e vira o anfitrião: a partida roda no seu aparelho.
- **Entrar:** os amigos digitam o código em *Entrar numa sala*, ou abrem o link que o anfitrião mandou (`?sala=CODIGO`).
- No 2×2 o parceiro senta na sua frente e a dupla soma os pontos das mãos adversárias. Toque numa vaga livre para trocar de lugar.
- No 2×2 e no Todos, vagas livres viram bots. Se alguém cair, um bot assume até a pessoa voltar com o mesmo nome.
- **Coringas e loja** (pode ser desligado ao criar a sala): cada um começa com $8 e escolhe 1 coringa. Depois de cada mão todos ganham $2, quem venceu ganha mais $3, e a loja abre para todos ao mesmo tempo. A mão seguinte começa quando todos tocam em *Pronto*.
- Vence quem chegar primeiro à meta de pontos.

A conexão é direta entre os navegadores (WebRTC, via [PeerJS](https://peerjs.com)). O servidor público do PeerJS só apresenta os jogadores uns aos outros; as jogadas não passam por ele. Precisa de internet, e o anfitrião deve manter a aba aberta.

## Jogar online (GitHub Pages)

Em **Settings → Pages**, escolha *Deploy from a branch*, depois a branch `main` e a pasta `/ (root)`. Em um ou dois minutos o jogo fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Estrutura

| Arquivo | O que é |
|---|---|
| `index.html` | O jogo inteiro: HTML, CSS e JavaScript (o PeerJS é carregado de um CDN só quando você abre o modo online) |

## Status

Protótipo em desenvolvimento (v0.6).
