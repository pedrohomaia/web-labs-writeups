# Write-up (Lab) — CSRF e cookies SameSite

## Contexto (Lab)
Tema educacional: ações sensíveis disparadas sem intenção do usuário quando há sessão via cookie.

## Como reconhecer (sinais)
- Endpoints state-changing sem token anti-CSRF
- Cookies sem SameSite adequado

## Impacto
- Mudança de email/senha, ações indesejadas se usuário estiver logado

## Mitigação
- Tokens anti-CSRF
- SameSite=Lax/Strict conforme caso
- Reautenticação para ações sensíveis

## Validação
- Confirmar que ações exigem token e/ou SameSite impede submissões cross-site
