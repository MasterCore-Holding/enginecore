# esteira/ — automações de funil

Registro das automações que operam a esteira de crescimento da EngineCore.

## Estado atual (27/10/2026)

| Etapa | Como funciona hoje | Onde vive |
|---|---|---|
| Captura | Formulário de qualificação em `qualificacao/` | Servido pelo GitHub Pages |
| Registro de lead | `registrarLeadAppsScript` grava no Google Apps Script | Script do grupo (fora deste repo) |
| Destino CRM | Espelho de leads no CRM do grupo | Fora deste repo |

## Fronteira

Nenhuma automação desta pasta executa operação de PeptiCore. A separação entre as
empresas do grupo é contratual (handoff formal + NDA) e técnica (workspaces
segregados), inclusive quando a esteira é a mesma.

Vedado, expressamente:
- Misturar dado de paciente/cliente de uma empresa com outra.
- Reaproveitar credencial de uma empresa em outra.

## Esteira compartilhada — o que isso significa

A EngineCore usa a mesma esteira técnica que a PeptiCore (é o argumento de
track record: "primeiro cliente, a própria casa"). Compartilhar tecnologia não
autoriza compartilhar dado. Cada empresa tem workspace próprio.

---
*Córtex (Control Plane) — 27/10/2026.*
