# site/ — landing enginecore.app

## Decisão de localização (27/10/2026): a landing NÃO mora aqui

O código da landing está na **raiz deste repositório** (`index.html`, `lander/`,
`qualificacao/`), e não nesta pasta.

Motivo: o GitHub Pages está configurado com `source = main / (raiz)`. Produção é
servida diretamente da raiz — **todo push em `main` é deploy**. Mover o HTML para
`site/` derrubaria enginecore.app no mesmo commit que o move, porque a configuração
de Pages aponta para a raiz.

Mover exigiria, na mesma janela: mudar a source do Pages para `main /site` (via UI
do GitHub — a API recusa com 403 no token atual) e mover os arquivos. Duas operações
acopladas, sem staging intermediário e sem rollback automático. Classificado como
**faixa amarela/vermelha** — não executado por agente.

## O que esta pasta é hoje

Ponto de extensão reservado. Quando a source do Pages for movida para cá (decisão do
CEO, com janela de deploy declarada), a landing passa a viver aqui e a raiz fica com
configuração e documentação.

## Regra enquanto isso

Todo caminho de landing em documentação aponta para a raiz. Não referencie
`site/index.html` — ele não existe.

---
*Córtex (Control Plane) — 27/10/2026.*
