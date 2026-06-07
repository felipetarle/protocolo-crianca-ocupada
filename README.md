# Protocolo Criança Ocupada — Landing

Landing page de vendas para o e-book **Protocolo Criança Ocupada** (R$57, Hotmart).

## Stack
- HTML estático single-file (`index.html`)
- Tailwind via CDN
- Google Fonts: Fraunces (títulos) + Poppins (corpo)
- Zero build step — abre direto no navegador

## Como rodar local

```bash
python3 -m http.server 8000
# abre http://localhost:8000
```

## Antes de publicar

1. Trocar `{{CHECKOUT_HOTMART_URL}}` pelo link do checkout (5 ocorrências em `index.html`)
2. Atualizar `<meta property="og:image">` com URL absoluta de produção
3. Opcional: comprimir `images/hero-mae-filhos.jpg` (hoje 212KB → WebP economiza ~50%)

## Estrutura
- `index.html` — página completa
- `images/hero-mae-filhos.jpg` — ilustração do herói (1280×720)

## Decisões de design
- Persona: mulher (mãe/avó/tia), classe C, tráfego frio de Meta Ads
- Copy inclusiva (cuidadores em geral) — "as crianças" em vez de "seus filhos"
- Paleta creme + coral CTA (`#E0532A`) + teal de oferta (`#2E6F63`)
- Value stack Hormozi: itens com preço cheio riscado, total R$255 → R$57 (77% off)
- Garantia incondicional 7 dias com dobra dedicada
- Mobile-first, CTA visível na primeira dobra
