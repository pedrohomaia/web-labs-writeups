# Write-up (Lab) — Security Headers (Básico)

## Contexto (Lab)
Tema educacional: hardening no navegador via headers.

## Como reconhecer (sinais)
- Respostas HTTP sem HSTS/CSP/Referrer-Policy etc.
- Páginas embutíveis por terceiros (risco de clickjacking)

## Impacto
- Maior superfície para ataques no browser
- Possíveis downgrades/embeds indevidos dependendo do contexto

## Mitigação
- HSTS bem configurado
- CSP adequada ao app
- X-Content-Type-Options, Referrer-Policy, Frame-ancestors (via CSP)

## Validação
- Confirmar headers presentes
- Testar fluxos críticos e ajustar política CSP se necessário
