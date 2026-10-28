# EngineCore — enginecore.app

Agência de performance operada por IA autônoma, com supervisão humana.

Não vendemos horas. Operamos uma esteira de crescimento: a IA executa, o humano
supervisiona nos gates, e todo relatório separa o que foi **proposto** do que foi
**aplicado**.

## Pacotes

| Pacote | Natureza | Modelo |
|---|---|---|
| Simples | Projeto pontual — landing page de alto padrão + automação de lead para WhatsApp | Fee fixo |
| Médio | Escopo dedicado e contínuo — conteúdo, automações profundas ou tráfego pago | Retainer mensal fixo |
| Top | Skin in the game — fee mínimo + verba de mídia + fatia do crescimento | Fee base + performance |
| Fundador | 3 a 5 primeiros clientes — fee reduzido, case público com métricas reais | Fee reduzido + upside |

Piso garantido: nenhum projeto fecha abaixo do piso. O fee de discovery (R$ 1.000)
é cobrado à frente e 100% creditado no fechamento — se não fechar, o cliente fica
com o diagnóstico de valor.

## Regra de relatório — Proposto ≠ Aplicado

Todo relatório entregue a cliente separa explicitamente:

- **Proposto** — o que foi planejado e aprovado.
- **Aplicado** — o que foi executado e verificado em runtime, com evidência.

Relatório que mistura os dois é considerado defeito, não estilo.

## Estrutura do repositório

| Caminho | Conteúdo |
|---|---|
| `index.html` | Landing principal — servida por GitHub Pages na raiz do domínio |
| `lander/` | Variante de landing |
| `qualificacao/` | Formulário de qualificação (topo do funil) |
| `docs/` | Documentação técnica e de operação |
| `esteira/` | Registro e código das automações de funil |
| `CHANGELOG.md` | Histórico de versões |
| `CNAME` | Domínio customizado do GitHub Pages |

## Deploy

GitHub Pages, branch `main`, raiz do repositório, domínio `enginecore.app`
(CNAME + HTTPS forçado, certificado aprovado).

**Produção é servida diretamente deste repositório: todo push em `main` é deploy.**
Alteração de conteúdo publicado exige PR — não há etapa de staging.

---
*EngineCore — empresa do Grupo MasterCore.*
