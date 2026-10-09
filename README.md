# Biblioteca Digital UniFECAF

Projeto acadêmico da disciplina **Design Web**: uma página de biblioteca digital moderna, responsiva e acessível, feita apenas com **HTML5 e CSS3**, a partir de um protótipo de baixa fidelidade.

- **Site publicado:** https://akta-sys.github.io/biblioteca-unifecaf/
- **Autor:** Guilherme Alves Cordeiro Barros

## Objetivo

Transformar o protótipo em uma interface funcional, mantendo a ordem das seções e a hierarquia visual, com:

- identidade visual inspirada na UniFECAF (paleta azul + verde de destaque, fonte Poppins);
- layout que se adapta a desktop e smartphone, sem texto cortado, imagens distorcidas ou sobreposições;
- princípios básicos de acessibilidade (HTML semântico, contraste, foco visível, textos alternativos).

## Estrutura do projeto

```
biblioteca-unifecaf/
├── index.html          # estrutura semântica da página
├── css/
│   └── style.css       # estilos (mobile-first) e responsividade
├── assets/
│   └── imagens/        # fotos otimizadas (JPG)
└── README.md
```

## Seções da página

1. Menu de navegação (Biblioteca, Livros, Unidades, Contatos)
2. Banner principal
3. Sobre a nossa biblioteca (texto, imagem e galeria)
4. Banner intermediário
5. Nossos livros (6 cards)
6. As unidades (3 blocos)
7. Contatos
8. Rodapé

## Decisões técnicas

- **Mobile-first:** estilos base para celular; `@media (min-width)` amplia para tablet (768px) e desktop (900px).
- **CSS Grid** nos cards de livros (`repeat(auto-fit, minmax(min(100%, 300px), 1fr))`) e **Flexbox** no menu.
- **Variáveis CSS** (`:root`) para paleta, fonte e medidas.
- **Imagens:** `max-width: 100%`, `aspect-ratio` e `object-fit: cover` evitam distorção.
- **Acessibilidade:** um único `<h1>`, `aria-labelledby` nas seções, link "Pular para o conteúdo", `:focus-visible`, `prefers-reduced-motion`.
- **Nomenclatura BEM** nas classes (`bloco__elemento--modificador`).

## Como executar

Não precisa de instalação. Baixe o repositório e abra o `index.html` no navegador.

## Créditos

- Fotografias: banco de imagens gratuito (uso livre).
- Fonte: [Poppins](https://fonts.google.com/specimen/Poppins), via Google Fonts.
- Contatos e unidades são **fictícios**, criados apenas para fins acadêmicos.
