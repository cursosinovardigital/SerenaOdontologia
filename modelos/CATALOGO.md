# Catálogo de modelos — github.com/cursosinovardigital

Levantamento feito em 11/11/2026. Os 16 repositórios da conta são **públicos**,
então dá para clonar de novo a qualquer momento, sem token:

```bash
git clone --depth 1 https://github.com/cursosinovardigital/<repositorio>.git
```

## Ranking de utilidade para a Serena Odontologia

1. **drcarolinaestetica** — clínica de harmonização facial, mesma área e mesmo público.
   Útil para comparar organização de procedimentos, tom de voz e a paleta quente
   (champanhe/bege) como alternativa ao verde da Serena.
2. **tenista-modelo-apresenta-** — arquitetura de seções muito próxima da que a Serena usa
   (hero, sobre, programas, instalações, números, depoimentos, contato), com números
   animados e navegação por pontos. Boa referência de ritmo de página longa.
3. **SiteCraft.io** — o mais completo em sistema de design: tokens de cor, cartões de
   vidro (`--bg-glass`, `--bd-hover`), catálogo de modelos e "montador". Referência para
   evoluir os componentes da Serena sem inventar padrão novo.
4. **lumura-apresenta-ao** — minimalismo editorial em preto e branco, grid de trabalhos e
   formulário de contato. Serve se a ideia for uma galeria de casos (antes/depois).
5. **ale-test** — landing local curta (serviço, prova real, avaliações, localização). Bom
   molde de página objetiva quando não há conteúdo para 7 seções.
6. **guarana-apresenta-o** — efeitos de vidro e animação com GSAP; referência de movimento.

## Tabela completa

| Repositório | O que é | Stack | Vale aproveitar |
|---|---|---|---|
| `SerenaOdontologia` | O site da clínica (este projeto) | HTML único, sem framework | Base atual; backup em `backup/` |
| `drcarolinaestetica` | Harmonização facial, Guarulhos | HTML único, Fraunces + Jost | Paleta champanhe, seções de procedimentos e resultados, depoimentos |
| `tenista-modelo-apresenta-` | Clube de tênis | HTML único + Lenis, Onest | Arquitetura de seções, contadores e depoimentos |
| `SiteCraft.io` | Estúdio/construtor de sites + catálogo | Tailwind, 4 fontes, sistema de tokens | Tokens de design, cartões de vidro, catálogo navegável |
| `lumura-apresenta-ao` | Estúdio de design (em inglês) | HTML único + Lenis, Onest | Minimalismo, grid de trabalhos, formulário |
| `ale-test` | Estética automotiva, Guarulhos | Tailwind | Landing curta de serviço local, prova real |
| `guarana-apresenta-o` | Landing de produto (Diet Soda) | GSAP, tema escuro | Glassmorphism e animação de rolagem |
| `infynix-model` | Agência de AI SDR/tráfego | HTML único, tema escuro + laranja | Seção "núcleo interativo", FAQ, blocos de solução |
| `kimi-antonelli-apresenta-o` | Site editorial de corrida (inglês) | Lenis, Oswald + Space Grotesk | Tipografia condensada, seções full-bleed |
| `laocoom-apresenta-o` | Página editorial sobre escultura (inglês) | HTML único, Playfair + Italiana | Composição editorial com serifada |
| `leftacademia` | Academia em Guarulhos | Tailwind, Anton + Inter | Tabela de planos, seção de app, depoimentos |
| `NextGenStore` | Loja tech com retirada em loja | Tailwind | Cartões de produto e CTA de WhatsApp |
| `Prospecta.io` | CRM de prospecção | Tailwind, JS com templates | Painel compacto, listas e funil |
| `Bilini-English-School` | Escola de inglês | Tailwind + GSAP | Página leve (21 KB) e ritmo enxuto |
| `cursosinovardigital` | Portal de cursos (20 páginas) | HTML multi-página, Inter | Navegação multi-página, cartões de curso |
| `lowticketlucrativo` | Landing de infoproduto | HTML, neon sobre escuro | Estrutura de oferta e prova de resultado |

## Cópias locais (offline)

Estão em `modelos/referencias/`, só o HTML principal de cada um — as imagens continuam
nos repositórios originais:

| Arquivo | Origem | Tamanho |
|---|---|---|
| `referencias/drcarolinaestetica.html` | `drcarolinaestetica` | 48 KB |
| `referencias/tenista-clube.html` | `tenista-modelo-apresenta-` | 82 KB |
| `referencias/sitecraft.html` | `SiteCraft.io` | 110 KB |
| `referencias/lumura.html` | `lumura-apresenta-ao` | 90 KB |

## Observações

- `leftacademia`, `cursosinovardigital` e `lowticketlucrativo` passam de 800 KB com imagens;
  não copiei para cá de propósito. Se algum virar base, clonar do GitHub.
- Nada aqui entra no site da Serena como está: são referências de estrutura, tipografia e
  movimento. Textos de outra clínica ou de outro negócio nunca devem ser reaproveitados.
- Modelos em inglês (`kimi`, `laocoom`, `lumura`) servem só de referência visual.
