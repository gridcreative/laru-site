# La.rú Arquitetura — Site institucional

Site estático de 4 páginas para a **La.rú Arquitetura** (São Paulo · SP), escritório de arquitetura corporativa e residencial das sócias Laís e Rúbia. Desenvolvido por **Grid & Grain Creative**.

## Estrutura

```
index.html      → Início (hero com slideshow de 5 imagens)
projetos.html   → Projetos (residencial + corporativo)
sobre.html      → Sobre nós
contato.html    → Contato (formulário ilustrativo — não envia e-mail)
styles.css      → Folha de estilos única, compartilhada pelas 4 páginas
img/            → Imagens (fotos geradas por IA + logos em .webp)
```

Sem build, sem dependências, sem framework: HTML + CSS + JavaScript puro. Basta servir a pasta com qualquer servidor estático (ex.: `python3 -m http.server`) ou abrir os arquivos no navegador.

O site é publicado via **GitHub Pages** a partir da branch `main` (raiz).

## Identidade visual

Definida como variáveis CSS em `:root` no `styles.css`:

| Token | Cor | Uso |
|---|---|---|
| `--nacar` | `#ECE8E2` | Fundo principal |
| `--linho` | `#C0BAAD` | Acentos (ponto do monograma, detalhes) |
| `--taipa` | `#3A3231` | Faixas escuras, textos |

- Tipografia: **Epilogue** (Google Fonts), pesos 200–500.
- A curva no canto das imagens (`border-top-right-radius`) e os pontos circulares ecoam o monograma "la.rú".

## Pontos de atenção

- **Formulário de contato** (`contato.html`): apenas visual; integrar com um backend ou serviço (Formspree, etc.) antes de ir ao ar.
- **Slideshow do hero** (`index.html`): troca automática a cada 5,5 s com crossfade; respeita `prefers-reduced-motion`.
- **Nomes de projetos** são ilustrativos (exceto "Apartamento Amauri").
- Instagram: <https://www.instagram.com/la.ruarquitetura/>
