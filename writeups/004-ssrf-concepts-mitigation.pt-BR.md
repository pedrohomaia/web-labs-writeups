# Write-up (Lab) — SSRF (conceito e mitigação)

## Contexto (Lab)
Tema educacional: servidor fazendo requisições para URLs controladas pelo usuário.

## Como reconhecer (sinais)
- Funcionalidades que “buscam URL”, “importam imagem”, “webhook”, “preview”
- Falta de validação de destino/host

## Impacto
- Acesso a recursos internos, enumeração interna, abuso de metadados cloud (dependendo do ambiente)

## Mitigação
- Allowlist de destinos (domínios) + validação robusta
- Bloquear IPs privados/metadata + resolver DNS com cuidado
- Egress firewall / redes separadas

## Validação
- Testar apenas em lab: confirmar que destinos não permitidos são bloqueados com segurança
