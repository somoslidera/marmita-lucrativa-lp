# Marmita Lucrativa, landing page

LP de vendas do app Marmita Lucrativa (R$ 47, pagamento único, Kiwify).
HTML estático único (`index.html`) + prints reais do app em `assets/`.

## Antes de publicar

1. **Link do checkout.** No fim do `index.html`, troque `CHECKOUT_URL`
   pelo link de pagamento do produto na Kiwify. Todos os botões de compra
   usam essa constante e repassam as UTMs da página para o checkout.
2. **Pixel da Meta (opcional).** Se quiser medir, cole o snippet do pixel
   no `<head>`. O clique de compra já dispara `InitiateCheckout` quando
   `fbq` existe na página.
3. **og:image.** Está apontando para `assets/og.jpg` (caminho relativo).
   Depois de publicar, troque pela URL absoluta do domínio final.

## Publicar

Mesmo caminho das outras LPs: Vercel ou GitHub Pages, a pasta inteira
(`index.html` + `assets/`). Nada de build.

## Atualizar os prints do app

Os prints vieram do app em modo local (sem nuvem) com a loja de exemplo
"Marmitaria do Bairro". Para refazer, abra o `Marmita-Lucrativa.html` com
`SUPA_URL=''`, navegue até a tela e capture em 1280 px (desktop) ou 390 px
(celular). Os números da seção "A conta" e do card do hero vêm dessa loja:
Marmita M · Carne moída (custo R$ 9,35) e Marmita G · Mista (custo R$ 11,53).
Se a loja de exemplo mudar, revise esses números no texto.
