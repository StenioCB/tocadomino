# tOca Dominó: página de entrada

Página estática, hospedada no GitHub Pages, que nunca dorme. Ela mostra uma tela amigável enquanto o servidor do jogo
(`https://tocadomino.onrender.com`, plano gratuito do Render) acorda, e depois leva o jogador ao jogo, mantendo o
código da mesa do convite (`?mesa=CODIGO`).

- O jogo gera os convites com o endereço desta página.
- Ela pergunta ao servidor, a cada 2 segundos, em `/healthz`, se já acordou.
- Depois de 75 segundos sem resposta, abre o jogo mesmo assim (a tela do próprio Render assume).
