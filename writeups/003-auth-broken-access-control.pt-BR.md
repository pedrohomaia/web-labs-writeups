# Write-up (Lab) — Broken Access Control (conceito e mitigação)

## Contexto (Lab)
Tema educacional: falhas de autorização quando backend não valida permissões corretamente.

## Como reconhecer (sinais)
- IDs previsíveis (IDOR) e ausência de checagem de owner/role
- Diferença entre controle no front-end vs validação no backend

## Impacto
- Acesso indevido a dados e ações (ex.: ler/alterar recursos de terceiros)

## Mitigação
- Checagem de autorização no servidor para cada ação
- Regras RBAC/ABAC centralizadas
- Logs/auditoria para ações sensíveis

## Validação
- Testar recursos de outro usuário (em lab) e garantir 403/negativa correta
