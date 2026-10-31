# Prompt: página de vendas do Guia da Pega (versão que não cai no filtro de saúde da Meta)

Crie uma landing page de vendas, mobile first (90% do tráfego vem do Instagram, navegador do app), de página única, leve e rápida, para o produto digital **Guia da Pega**, da Dayane dos Anjos (Manual do Recém-Nascido).

## Contexto e restrição principal (leia antes de escrever qualquer texto)

A Meta classifica sites pelo assunto do texto. Se ela entender que a página trata de **condição médica, sintoma, lesão, tratamento ou relação profissional de saúde e paciente**, o domínio é marcado como "saúde e bem-estar" e o pixel para de receber checkout e compra. A página anterior caiu nesse filtro em 13 dias porque falava de dor, fissura, seio machucado, ingurgitamento, enfermeira e consultora.

Esta página precisa vender a mesma coisa falando de **técnica, aprendizado, rotina e vínculo**, nunca de sintoma ou cura.

### Palavras e assuntos PROIBIDOS no texto visível, no título da aba, nas metas (title, description, og:*), nos alt das imagens e nos nomes de arquivo

dor, doer, dói, dolorido, fissura, rachadura, ferida, machucado, machucar, sangrar, sangramento, carne viva, cicatrizar, lesão, inflamação, infecção, mastite, ingurgitamento, leite empedrado, bico de silicone, pomada, remédio, tratamento, tratar, curar, cura, sintoma, diagnóstico, médico, pediatra, enfermeira, consultora de amamentação, profissional de saúde, paciente, clínica, hospital, saúde, problema de saúde, "corrigir" a amamentação.

### Como reescrever (troque o sintoma pelo resultado positivo e concreto)

| Em vez de | Escreva algo como |
|---|---|
| Amamentar dói? A dor vai embora | Mamadas tranquilas desde a próxima vez que você oferecer o peito |
| Sem fissura e sem bico de silicone | Do jeito natural, só com você e o seu bebê |
| Seio machucado / em carne viva | Quando a mamada não está do jeito que você imaginava |
| Corrija a amamentação | Aprenda a pega certa, passo a passo |
| O que fazer com fissura | Como deixar cada mamada mais confortável |
| Leite empedrado / produção | Como organizar as mamadas ao longo do dia |
| Enfermeira / consultora | Dayane, mãe e criadora do Manual do Recém-Nascido, que já ensinou milhares de mães |

Tom: conversa de mãe pra mãe, acolhedor e prático, primeira pessoa da Dayane. Frases curtas. Sem travessão (— ou –), use vírgula, ponto ou dois pontos. Sem emoji de mamadeira. Emojis permitidos com moderação: 🤱 💛 🤍.

## Estrutura (mantém a ordem da página que converte, só troca o enfoque)

1. **Topo (primeira tela, sem rolar):** headline curta sobre mamadas tranquilas e a pega certa + subtítulo dizendo que é um passo a passo em vídeo com bebê de verdade + **foto da Dayane amamentando ou com bebê** + **botão de compra já na primeira tela** (não use botão "role para entender"). Selo pequeno: "Aulas práticas com bebê de verdade".
2. **"Você se reconhece aqui?"**: 4 ou 5 situações descritas como desejo ou insegurança, nunca como sintoma. Ex: "Você fica na dúvida se o bebê está mamando direito", "Cada mamada parece uma luta e você queria curtir esse momento", "Você ouve um conselho diferente de cada pessoa".
3. **A virada:** existe um jeito de oferecer o peito que deixa a mamada mais fácil pra você e pro bebê. O segredo é a pega, e pega se aprende.
4. **Quem ensina:** Dayane dos Anjos, mãe, criadora do Manual do Recém-Nascido (mais de 600 mil seguidoras). Sem títulos de profissional de saúde.
5. **O que você vai aprender:** lista em tópicos curtos (posição, como oferecer o peito, como saber que a pega está certa, como o bebê sinaliza que está satisfeito, ritmo das mamadas, como deixar cada mamada confortável).
6. **Depoimentos:** 3 ou 4 em formato de print de conversa, falando de resultado e emoção ("agora a mamada virou o nosso momento", "ela mama tranquila e dorme satisfeita"). Nenhuma descrição de lesão ou sintoma.
7. **Bônus inclusos** (renomeados): "Como saber se o bebê está mamando bem" · "Como deixar cada mamada mais confortável" · "Como organizar as mamadas ao longo do dia" · "O que fazer quando o peito fica cheio demais".
8. **Oferta:** perto do preço, repetir em lista curta tudo o que a pessoa leva (aulas + 4 bônus). Preço: **de R$ 97 por R$ 67 à vista ou em até 12x de R$ 6,89**. Botão: "Quero aprender a pega certa". Abaixo: 🔒 7 dias de garantia · Acesso imediato · Compra 100% segura.
9. **Como funciona:** 1) compra com acesso imediato 2) acesso chega no e-mail 3) assiste e aplica na próxima mamada.
10. **Perguntas frequentes** (5 a 6): para quem é, quando posso começar, por quanto tempo tenho acesso, e se eu não gostar (garantia), serve pra qualquer idade do bebê. Sem perguntas sobre sintoma.
11. **Botão final** + rodapé simples (marca, contato, links de termos e privacidade).

Botões de compra em pelo menos 3 pontos: topo, depois do "o que vai aprender" e na oferta.

## Técnico (obrigatório)

- **Link de checkout de todos os botões** (classe `btn-comprar`):
  `https://payfast.greenn.com.br/136511/offer/sP4rpP?ch_id=24103&b_id_1=119667&b_offer_1=5MBzpG&b_id_2=119638&b_offer_2=zrQIbg`
- **Repassar ao checkout** todos os parâmetros da URL que começam com `utm_`, mais `fbclid`, e os cookies `_fbp` e `_fbc` (como `fbp` e `fbc`). Sem isso a venda não casa com a campanha.
- **Meta Pixel** com o ID `<PIXEL_ID_NOVO>`: `PageView` e `ViewContent` (value 67, BRL) ao carregar, e `InitiateCheckout` (value 67, BRL) no clique de qualquer `btn-comprar`, esperando cerca de 250 ms antes de ir para o checkout. Usar `eventID` em cada evento.
- **Microsoft Clarity** com o ID `<CLARITY_ID>`.
- Imagens em WebP, com largura e altura definidas e carregamento tardio fora da primeira tela. Alvo: carregar em menos de 2,5 s no 4G.
- Nada de texto escondido, palavra-chave repetida ou truque para enganar a Meta. A página precisa ser limpa de verdade.
- Entregar como HTML estático único (com CSS e JS inline), pronto para GitHub Pages.

## Antes de entregar, confira

1. Busque no HTML inteiro cada palavra da lista proibida (inclusive no `<title>`, nas metas, nos `alt` e nos nomes de arquivo). O resultado precisa ser **zero**.
2. Teste os botões: o link de checkout precisa sair com `utm_*`, `fbclid`, `fbp` e `fbc` quando a página é aberta com esses parâmetros.
3. Confira no celular que headline, foto e botão aparecem na primeira tela sem rolar.
