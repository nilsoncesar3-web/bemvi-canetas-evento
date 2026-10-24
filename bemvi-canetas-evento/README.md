# Aula aberta: Canetas emagrecedoras e saúde mental

Material de divulgação e inscrição do evento **Bemvi Hands-On | Aula Aberta**, do BemviHub.

- **Data:** sábado, 28/11, às 15h
- **Local:** Auditório do Centro Empresarial, Shopping Rio Poty (presencial)
- **Palestrante:** Dr. Luis Fábio, psiquiatra (CRM 8306 | RQE 6234)

## Estrutura

| Pasta | Conteúdo |
|---|---|
| `inscricao/index.html` | Formulário de inscrição (página única, abre direto no navegador) |
| `post/` | Fonte da arte do post 1080×1080 (`Main.dc.html`, `canvas.json`) e `assets/` com fotos, logo e arte original |
| `docs/` | Perguntas do formulário e mensagens prontas de WhatsApp |

## Valores de inscrição

| Categoria | Valor |
|---|---|
| Acadêmico ou estudante da área da saúde | R$ 15 |
| Profissional de saúde formado | R$ 20 |
| Profissional do Instituto Bemvi | Gratuito |
| Profissional do Centro Empresarial do Shopping Rio Poty | Gratuito |

## Como o formulário funciona

O formulário não usa servidor. Ao finalizar, ele monta um resumo e abre o WhatsApp da Bemvi com a mensagem pronta; quem paga envia o comprovante do PIX na mesma conversa. As configurações ficam no objeto `CFG`, no final de `inscricao/index.html`:

```js
var CFG={whatsapp:"(86) 98188-9999",email:"[E-MAIL]",pix:"58.186.422/0001-83",favorecido:"Instituto Bemvi"};
```

Para testar, abra `inscricao/index.html` no navegador. Para publicar, hospede a pasta `inscricao/` em um serviço de páginas estáticas (GitHub Pages, Netlify, Cloudflare Pages ou o site do Instituto Bemvi).

## Observações

- A arte em `post/Main.dc.html` referencia imagens do ambiente do Claude (`/_blob/...`). Para editar fora de lá, use os arquivos de `post/assets/` e exporte a imagem final em 1080×1080.
- Comunicação médica: seguir as regras de publicidade do CFM (Resolução CFM 2.336/2023). Não citar marcas nem prometer resultados.
