# Write-up (Lab) — SQLi (conceito e mitigação)

## Contexto (Lab)
Tema educacional: injeção em consultas quando entrada não é tratada com segurança.

## Como reconhecer (sinais)
- Erros de banco/consultas
- Comportamento diferente ao variar parâmetros
- Falhas de validação e ausência de queries parametrizadas

## Impacto
- Vazamento/alteração de dados
- Bypass de autenticação (dependendo do contexto)

## Mitigação
- Queries parametrizadas/prepared statements
- Validação de entrada (tipo, formato, limites)
- Menor privilégio no usuário do DB

## Validação
- Re-testar endpoints e garantir que entradas não alteram lógica de consulta
