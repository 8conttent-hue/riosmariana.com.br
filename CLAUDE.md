# CLAUDE.md — RIOSMARIANA

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** RIOSMARIANA
**Nicho:** Viagens e Turismo
**Keywords:** Acho que a paixao por viagens carreiras crescimento profissional e moda foram
**Paleta de cores:** rose | **Fonte:** playfair

Acho que a paixão por viagens, carreiras, crescimento profissional e moda foram os responsáveis pela ideia. Por gostar muito, e estar trabalhando diariamente nesses aspectos, surgiu a ideia postar conteúdos com dicas detalhadas e informações. Quando estou escrevendo, imagino todas as pessoas lendo e tendo conhecimentos que agreguem nas suas vidas, então tento ser o mais clara possível, dando boas dicas. Obrigado desde já 🙂



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-J |
| Hero | Hero-C |
| Features | Features-H |
| About Section | About-B |
| Posts | Posts-A |
| Footer | Footer-G |
| Página Sobre | Sobre-C |
| Página Contato | Contato-E |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
