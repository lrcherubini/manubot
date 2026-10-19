# Vão Livre

Jogo de plataforma de precisão (PWA) publicado via GitHub Pages.

## Publicação
O workflow `.github/workflows/pages.yml` publica o site a cada push em `main` (ou no branch de desenvolvimento).
Uma única vez: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

## Offline
`sw.js` pré-carrega todos os arquivos (HTML, ícones, manifest e fontes auto-hospedadas em `fonts/`).
O botão de download no HUD mostra o estado: ✓ pronto para jogar offline, botão dourado = nova versão disponível.
**A cada deploy, incremente `VERSION` em `sw.js`** para os jogadores receberem a atualização.
