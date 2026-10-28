# assets/ — ativos estáticos

## Estado atual (27/10/2026): ativos referenciados na raiz

Os ativos usados pela landing estão na raiz do repositório, ao lado do HTML que os
referencia: `logo-enginecore*.png/webp`, `favicon-*.png`, `apple-touch-icon.png`.

Isso não é desorganização — é consequência da configuração de Pages (`source = main /
raiz`). Os caminhos no HTML são relativos, então mover um ativo para `assets/` sem
editar todos os `src=` quebra a imagem em produção no mesmo push.

## Convenção para ativos novos

Ativo novo que ainda **não** está referenciado em HTML publicado entra aqui, com nome
descritivo em kebab-case e o formato de menor peso que atenda o uso (webp para foto,
png/svg para marca com transparência, jpg para foto opaca).

Ao promover um ativo desta pasta para a raiz, o commit que o move atualiza todas as
referências no mesmo commit. Nunca em dois commits.

## Peso

Ativo acima de 300 KB precisa de justificativa no commit — a landing tem meta de
Lighthouse ≥ 90 no mobile, e imagem é o gargalo mais comum.

---
*Córtex (Control Plane) — 27/10/2026.*
