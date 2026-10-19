# Manubot

Robô de manutenção numa fábrica em pane. Plataforma de precisão com setores procedurais (PWA), publicada via GitHub Pages.

## Como jogar
- Repare o **terminal** para ligar o **teleporte** e escape do setor.
- A bateria do Manubot é o cronômetro: **células de energia** dão +2 s.
- Queda alta causa **sobrecarga** (−5 s e um breve curto-circuito). No **Insano** continua fatal.
- Perigos: bobinas de alta tensão, serras em trilhos (o trilho mostra a rota), prensas hidráulicas, torretas de míssil (com linha de mira) e lasers de solda.
- **Setores em sequência**: cada vitória avança o setor; pular a fase ou trocar a dificuldade zera a sequência. O recorde por dificuldade fica salvo no aparelho.
- **Compartilhar**: todo setor tem um código (`?s=CODIGO&d=DIFICULDADE`); o botão Compartilhar envia o link.
- Teclado: ← → / A D mover · Espaço/↑ pular · R reinicia · N novo setor · M som. Toque: metade esquerda arrasta para mover, direita pula.

## Publicação
O workflow `.github/workflows/pages.yml` publica o site a cada push em `main`.
Uma única vez: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

## Offline
`sw.js` pré-carrega todos os arquivos (HTML, ícones, manifest e fontes auto-hospedadas em `fonts/`).
**A cada deploy, incremente `VERSION` em `sw.js`** para os jogadores receberem a atualização.
