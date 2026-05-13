# Plano de Lançamento — Convites Digitais Sua Retrospectiva

## 1. Diagnóstico estratégico

### O problema central que esse plano resolve
Você identificou que clientes de **retrospectiva** chegam na semana da festa. Convite é o oposto: cliente precisa **30-60 dias antes**. Se você usar a mesma estratégia das duas, vai falhar — ou paga mais caro pelo lead, ou captura tarde demais.

### A mudança de mentalidade
- **Retrospectiva** = produto de urgência. Você vende para quem **lembrou em cima da hora**.
- **Convite** = produto de planejamento. Você vende para quem **acabou de decidir fazer a festa**.

Por isso, na página de convites, o tom é "comece com o pé direito", não "última chance". O gatilho não é urgência: é **boa organização**.

---

## 2. O que foi implementado no site

### Arquivos
- `index.html` (atualizado) — sua página original com:
  - Link "✉️ Convites" na navbar
  - Faixa de cross-sell antes do CTA final apontando para convites
  - Footer com navegação entre as duas páginas
- `convites.html` (novo) — landing page dedicada a convites

### Estrutura da nova página convites.html
1. **Hero** — "O convite é a primeira emoção da sua festa" + mockup visual de envelope/convite
2. **Prova emocional** — narrativa do convite chegando no WhatsApp
3. **Três tipos de convite** (Estático / Animado / Interativo) com features de cada um
4. **Linha do tempo "Quando contratar"** — **a peça-chave do funil**, que educa sobre antecedência e converte planejamento em urgência positiva
5. **Quem faz (Gabi)** — herdando autoridade já construída
6. **Como funciona** (4 passos)
7. **Pacotes** com 4 tiers (Essencial R$39,90 → Completo R$179,90)
8. **Diferenciais** (6 cards)
9. **Ocasiões atendidas** (pills com 11 tipos de festa)
10. **FAQ** específico de convites (7 perguntas)
11. **Cross-sell para retrospectiva** — captura lead pro outro produto
12. **CTA final + Fale conosco + Footer**

### Por que essa estrutura funciona
- **Quality Score alto no Ads**: página 100% sobre convites = relevância máxima → CPC mais barato
- **SEO independente**: rankeia para "convite digital", "convite animado", "convite interativo RSVP" sem competir com sua página de retrospectiva
- **Conversão otimizada**: a Timeline de antecedência educa o lead que chegou cedo e converte ele, em vez de deixar ele "voltar depois"
- **Cross-sell duplo**: tráfego de convite descobre retrospectiva e vice-versa, aumentando ticket médio

### O que você precisa ajustar manualmente antes de subir
1. **Formulário**: criar `formulario.html` aceitando o parâmetro `?produto=convite&pacote=X` (ou ajustar o existente para detectar o produto)
2. **Imagens/exemplos**: assim que tiver 3-6 exemplos reais de convite criados, substituir o mockup do envelope no hero por carrossel/grid com casos reais. Isso vai dobrar a conversão.
3. **JS de tracking**: o pixel Google Ads (`AW-18093869167`) já está no `<head>` herdado. Configure conversões separadas para retrospectiva e convite (instruções no item 5 abaixo).

---

## 3. Estratégia geral para captação antecipada

### Princípio: três frentes de captura
O cliente do convite passa por três momentos. Você precisa estar presente em cada um:

| Momento | O que o cliente faz | Sua presença |
|---|---|---|
| **Decidiu fazer festa** (45-60 dias antes) | Busca inspiração: "ideias de festa", "tema X", "como organizar" | Conteúdo + ads de descoberta |
| **Pesquisando convite** (30-45 dias antes) | Busca: "convite digital", "convite animado [tema]" | Ads de search com alta intenção |
| **Quer comprar agora** (15-30 dias antes) | Busca preço, compara, decide | Ads de search + remarketing |

### Lead magnet — captura quem ainda não vai comprar hoje
Você precisa de uma forma de capturar contato de quem está pesquisando **muito cedo** (50+ dias antes) e ainda não está pronto para comprar. Minha sugestão:

**"Checklist gratuito: 60 dias para uma festa sem stress"** — PDF de 1 página com cronograma do que fazer em cada semana antes da festa. Captura nome + email + WhatsApp + data da festa. Você tem o lead 60 dias antes, manda nutrição (1 email por semana) e na semana certa, oferece o convite. Em troca de zero esforço extra de tráfego.

---

## 4. Google Ads — Estrutura completa de campanha

### Configuração geral
- **Tipo**: Pesquisa (Search) — comece por aqui, é onde o lead com intenção alta está
- **Lance**: comece com "Maximizar cliques" por 2 semanas para ganhar dados, depois migre para "Maximizar conversões" (precisa de no mínimo 30 conversões por mês para isso funcionar bem)
- **Orçamento sugerido inicial**: R$25-40/dia (R$750-1.200/mês). Você está faturando ~R$6-7k em retrospectiva, então tem fôlego para testar
- **Localização**: comece com Brasil inteiro. Se descobrir que vendas se concentram em SP, refina depois
- **Idioma**: Português
- **Públicos**: mulheres 25-55 (perfil principal de organizador de festa familiar)

### Estrutura: 4 campanhas separadas

Por que separar? Porque cada uma tem intenção e CPC diferentes. Misturar tudo é desperdício de orçamento.

#### **CAMPANHA 1: Convite Digital — Genérico**
Captura intenção comercial direta.

**Grupos de anúncios:**
- *Convite digital* (correspondência: convite digital, convite digital animado, convite digital com RSVP)
- *Convite animado* (convite animado, convite animado para festa, convite virtual animado, convite animado WhatsApp)
- *Convite interativo* (convite interativo, convite com confirmação de presença, convite com RSVP, convite com link)

**Palavras-chave negativas (essenciais — adicione antes de subir):**
```
grátis, gratuito, free, canva, photoshop, illustrator, baixar, download, 
modelo, template, editar online, fazer, criar, app, programa, tutorial, 
como fazer, passo a passo, curso, aula
```
Isso filtra quem quer fazer sozinho ou está pesquisando tutorial — não é seu cliente.

#### **CAMPANHA 2: Convite por Ocasião**
Captura quem busca por tipo de festa. CPC tende a ser menor que termo genérico.

**Grupos de anúncios:**
- *Aniversário infantil* (convite aniversário infantil digital, convite festa infantil animado, convite 1 ano, convite 2 anos, convite 5 anos, etc.)
- *15 anos* (convite 15 anos animado, convite debutante digital, convite 15 anos interativo)
- *Casamento* (convite casamento digital, convite casamento animado, save the date digital)
- *Chá de bebê / revelação* (convite chá de bebê digital, convite chá revelação animado, convite chá de fraldas)
- *Outros* (convite batizado digital, convite formatura digital, convite bodas digital)

#### **CAMPANHA 3: Convite por Tema (Long-tail)**
Tema é onde mora ouro barato. CPC baixo, alta conversão.

**Grupos de anúncios:**
- *Temas infantis populares*: convite tema patrulha canina, convite tema lol surprise, convite tema super heróis, convite tema princesas, convite tema dinossauro, convite tema fazendinha, convite tema unicórnio, convite tema bluey
- *Temas adultos*: convite tema neon, convite tema boho, convite tema festa anos 80, convite tema tropical

A cada novo trabalho com tema específico, adicione o tema na lista. Esse é o "fundo do funil" — quem busca "convite tema bluey" tá quase comprando.

#### **CAMPANHA 4: Remarketing**
Para quem visitou `convites.html` e não converteu.

- Configure listas de remarketing no Google Ads vinculadas ao GA4 (ou pixel Google Ads).
- Lista 1: visitou convites.html, não enviou formulário, últimos 30 dias
- Lista 2: visitou pacotes (rolou até #pacotes) e não converteu, últimos 14 dias
- Anúncio: oferta de R$20 OFF ou "Última semana com desconto"

### Copy dos anúncios — 3 versões para teste A/B

**Versão A — Foco em diferenciação**
- Título 1: Convite Digital Personalizado
- Título 2: Animado, Interativo ou Estático
- Título 3: Feito à Mão, Não é Template
- Descrição 1: Encante seus convidados antes da festa começar. Vídeo, RSVP, mapa e contagem regressiva.
- Descrição 2: Entrega rápida + revisão inclusa. Atendimento direto com a criadora.

**Versão B — Foco em RSVP/funcionalidade**
- Título 1: Convite Digital com RSVP
- Título 2: Confirmação Automática
- Título 3: Convite Animado para WhatsApp
- Descrição 1: Receba as confirmações em tempo real num painel só seu. Sem mais perguntar um por um.
- Descrição 2: A partir de R$39,90. Entrega em até 4 dias úteis.

**Versão C — Foco emocional/antecedência**
- Título 1: Sua Festa Merece Começar Bem
- Título 2: Convite Digital Personalizado
- Título 3: Encante Antes da Festa
- Descrição 1: O convite é a primeira impressão da festa. Faça com carinho, do jeito que você imaginou.
- Descrição 2: Estático, Animado ou Interativo. A partir de R$39,90.

**Extensões para todos os anúncios:**
- *Sitelinks* (4): Convite Animado | Convite Interativo | Pacotes | Fale no WhatsApp
- *Frases de destaque*: "Entrega rápida" • "Revisão inclusa" • "Atendimento 1 a 1" • "Sem pagamento no site"
- *Snippets estruturados*: tipos = Estático, Animado, Interativo, Completo

### Lances iniciais (CPC manual para começar)
- Campanha Genérico: R$1,50-2,50 (mais competitivo)
- Campanha Ocasião: R$0,80-1,80
- Campanha Tema: R$0,50-1,20 (long-tail, barato)
- Remarketing: R$0,80-1,50

Depois de 2-3 semanas com dados, migre para "Maximizar conversões" e deixa o Google otimizar.

---

## 5. Configuração de conversões separadas (essencial!)

Para você saber qual campanha está performando, configure **duas conversões diferentes** no Google Ads:

1. **Conversão "Lead Retrospectiva"**: dispara quando alguém envia o formulário com `?produto=retrospectiva` (ou sem parâmetro = padrão retrospectiva)
2. **Conversão "Lead Convite"**: dispara quando envia formulário com `?produto=convite`

No código do formulário, adicione no momento do submit bem-sucedido:

```javascript
// Detecta qual produto
const urlParams = new URLSearchParams(window.location.search);
const produto = urlParams.get('produto') || 'retrospectiva';

// Dispara conversão correta
if (produto === 'convite') {
  gtag('event', 'conversion', {'send_to': 'AW-18093869167/COLE_ID_CONVITE_AQUI'});
} else {
  gtag('event', 'conversion', {'send_to': 'AW-18093869167/COLE_ID_RETROSPECTIVA_AQUI'});
}
```

Você pega os IDs criando duas ações de conversão diferentes no painel do Google Ads (Ferramentas > Conversões > Nova ação > Site).

---

## 6. Estratégias complementares que multiplicam o ROI

### Instagram orgânico — gratuito, alto impacto
- Poste 1 convite animado pronto por semana (caso real, com permissão). Reels com som dão muito alcance pra esse tipo de conteúdo.
- Hashtags: #conviteanimado #convitedigital #conviteaniversario #convite[tema]
- Stories: "antes e depois" do convite, processo de criação

### Parcerias locais (especialmente em SP)
Como você é de SP, contate buffets infantis, decoradores, fotógrafos e doceiras. Ofereça **20% de comissão** por indicação. Esse é o canal mais barato de aquisição para esse mercado — 1 buffet bem posicionado pode mandar 5-10 leads/mês.

### Funil de email/WhatsApp pós-lead-magnet
Quem baixar o "Checklist 60 dias" entra numa sequência automática:
- Dia 0: PDF + boas-vindas
- Dia 3: "Como escolher o tema da festa" (conteúdo)
- Dia 7: "5 erros ao escolher convite" (conteúdo + CTA leve pros pacotes)
- Dia 14: "Próximo passo: o convite" (CTA direto)
- Dia 21: depoimento de cliente + oferta especial
- Dia 30: última chamada

Você pode rodar isso de graça com Mailchimp (até 500 contatos) ou Brevo (até 300 emails/dia grátis).

---

## 7. Metas realistas para os primeiros 90 dias

Considerando seu faturamento atual de R$6-7k/mês só em retrospectiva, e adicionando convite:

| Período | Meta de leads/mês | Meta de vendas/mês | Faturamento adicional |
|---|---|---|---|
| Mês 1 (aprendizado) | 30-50 leads convite | 5-8 vendas | R$400 - R$1.000 |
| Mês 2 (otimização) | 60-90 leads | 12-18 vendas | R$1.000 - R$2.500 |
| Mês 3 (escala) | 100-140 leads | 20-30 vendas | R$2.000 - R$4.500 |

**Ticket médio esperado** com mix dos 4 pacotes: ~R$110-130.

Soma com retrospectiva, você tem potencial de R$8k-12k no terceiro mês. E o melhor: cliente de convite que vira recorrente (faz festa pro filho, depois do outro filho, depois bodas) é ouro.

---

## 8. Checklist de execução — em ordem

- [ ] Subir `convites.html` no servidor
- [ ] Substituir `index.html` pelo novo (com navbar atualizada + cross-sell)
- [ ] Ajustar `formulario.html` para aceitar `?produto=convite&pacote=X`
- [ ] Criar 2 ações de conversão no Google Ads (Lead Retrospectiva + Lead Convite)
- [ ] Adicionar JS de tracking diferenciado no submit do formulário
- [ ] Criar PDF "Checklist 60 dias para festa sem stress" (1-2 horas no Canva)
- [ ] Criar landing simples de captura do lead magnet (pode ser um pop-up no convites.html)
- [ ] Criar Campanha 1 (Genérico) no Google Ads — começa com R$15/dia
- [ ] Criar Campanha 2 (Ocasião) — R$10/dia
- [ ] Após 2 semanas: avaliar performance, adicionar Campanha 3 (Tema) e 4 (Remarketing)
- [ ] Postar 1 convite animado real por semana no Instagram
- [ ] Contatar 5 buffets/decoradores locais com proposta de parceria

---

## 9. O que monitorar semanalmente

- **CPC médio por campanha** (meta: cair com o tempo conforme Quality Score sobe)
- **CTR dos anúncios** (meta: >3% para search)
- **Taxa de conversão da landing** (meta inicial: 3-5%, ideal: 6-8%)
- **CPL — custo por lead** (meta: <R$15 para convite, dado o ticket médio)
- **CAC — custo por cliente** (meta: <R$40, ROI 3x)
- **Tempo entre primeiro contato e compra** (vai te dizer se está pegando lead cedo ou tarde)

---

## Considerações finais

A página está pronta para subir. Os preços que sugeri estão na faixa competitiva mas com margem para você ajustar conforme reação do mercado — se vender muito Essencial, sobe pra R$49,90. Se Interativo emperrar, baixa pra R$119,90 e ganha volume.

O ponto mais importante de tudo isso, repito: **a Timeline da página convites.html é o que vai te diferenciar.** Nenhum concorrente educa o cliente sobre antecedência dessa forma. Esse é seu ataque ao problema central que você levantou — gente chegando tarde.
