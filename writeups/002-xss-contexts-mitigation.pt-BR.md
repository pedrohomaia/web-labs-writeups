# Write-up (Lab) — XSS (contextos e mitigação)

## Contexto (Lab)
Tema educacional: injeção de script no navegador quando saída não é devidamente escapada.

## Como reconhecer (sinais)
- Input refletido/armazenado aparecendo no HTML
- Falta de escaping/encode por contexto (HTML, atributo, JS, URL)

## Impacto
- Roubo de sessão (dependendo de flags), ações em nome do usuário, defacement

## Mitigação
- Encode/escape por contexto
- Templates seguros e sanitização
- CSP bem desenhada para reduzir impacto

## Validação
- Testar entradas em múltiplos contextos e confirmar que aparecem escapadas
