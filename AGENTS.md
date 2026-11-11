# Serena Odontologia — notas do projeto

Site institucional de página única da Serena Odontologia (Centro de Guarulhos/SP).

## Stack

- `index.html` único: CSS e JavaScript inline, sem build, sem dependências.
- Imagens pequenas embutidas em base64 (logos do topo e do rodapé, foto do hero) para não depender de requisições externas.
- Publicação: GitHub Pages a partir da branch `main` — https://cursosinovardigital.github.io/SerenaOdontologia/
- Pages leva cerca de 1 minuto para reconstruir e manda `cache-control: max-age=600`, então quem já visitou pode ver a versão anterior por até 10 minutos.

## Convenções

- Todo o conteúdo em pt-BR.
- Cores da marca em `:root`: `--t1:#5cc1b9`, `--t2:#1a9488`, `--t3:#0d6b62`, `--bg2:#f1faf9`, `--bd:#d6ece9`, `--tx:#16302e`, `--mut:#51706d`.
- Tema escuro existe via `[data-theme="dark"]` e `prefers-color-scheme`; qualquer componente novo precisa funcionar nos dois.
- Fotos ficam em `assets/`, sempre WebP (qualidade 82, lado maior até 1440 px), otimizadas com Pillow.
- Usar somente fotos reais da clínica/equipe; fotos de pacientes só com autorização e nunca puxadas de redes sociais.
- Contato/CTA: WhatsApp `https://wa.me/5511992608891`, telefone (11) 4574-1704.
- Classes de componente existentes: `.card`, `.ic`, `.chips`, `.tm`, `.av`, `.grid`, `.hd`, `.rv0` (revelação por IntersectionObserver), `.car-*` (carrossel da equipe).

## Estrutura

- `index.html` — o site completo.
- `backup/index-v1-original.html` — modelo original antes das melhorias, preservado intacto como referência.
- `modelos/` — modelos de site/página de referência guardados para reaproveitar (ver `modelos/LEIA-ME.md`).
- `artifacts/` — prints de verificação gerados durante o trabalho; não versionado.
- `assets/` — fotos usadas pelo site.

## Fluxo de trabalho

- Servir localmente: `python3 -m http.server 3000 --bind 0.0.0.0`.
- Alteração só aparece no site publicado depois de commit e push na `main`; sempre avisar isso ao dono do projeto.
- Depois de mexer no CSS, conferir o resultado no navegador em viewport de celular (a maior parte do tráfego é mobile).
