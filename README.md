# 🌐 Detilli Hub — Documentação Completa

> Coleção de jogos e ferramentas web criados por Michel Detilli com a ajuda do replit**Detilli Hub**, hospedados no GitHub Pages.  
> 100% offline · sem instalação · mobile-friendly · código único por arquivo HTML.

---

## 📂 Estrutura de Arquivos no GitHub Pages

| Arquivo no GitHub | Descrição |
|---|---|
| `index.html` | Hub central com menu para todos os apps |
| `futebol.html` | Jogo World Penalty Champion |
| `cilada.html` | Jogo CILADA! (puzzle de peças) |
| `misterios.html` | Jogo Mistérios em Série |
| `foto-emoji.html` | Ferramenta Foto → Emoji |

> **Como subir:** cada arquivo `.txt` entregue pelo Replit deve ser renomeado para `.html` e enviado ao repositório do GitHub Pages.

---

## 🏠 Hub Central — `index.html`

Página inicial do Detilli Hub com menu visual para todos os aplicativos.

**Funcionalidades:**
- Cards visuais com prévia, descrição e tags de cada app/jogo
- Links diretos para cada ferramenta/jogo
- Design responsivo (mobile e desktop)
- Fundo animado com gradientes e efeito glow
- Rodapé com branding Detilli Hub

---

## ⚽ World Penalty Champion — `futebol.html`

Simulador de torneio de pênaltis mobile-first.

**Funcionalidades:**
- Arraste para mirar e solte para chutar
- Goleiro com IA animada que defende em direções aleatórias
- Sistema de pontuação acumulada
- Torneio progressivo por fases
- Efeitos visuais de gol e defesa
- Totalmente touch-friendly

---

## 🧩 CILADA! — `cilada.html`

Jogo de puzzle com peças poliominó (tipo Tetris, mas estático).

**Funcionalidades:**
- Tabuleiro 8×8
- Peças aleatórias geradas a cada partida
- Toque para selecionar peça → toque no tabuleiro para colocar
- Preview visual em verde (pode colocar) ou vermelho (não cabe)
- Botão **↻ Girar** (4 rotações únicas)
- Botão **↩ Desfazer** última jogada
- Detecção de **VITÓRIA** (todas as peças colocadas)
- Detecção de **CILADA** (sobram peças mas nenhuma encaixa em nenhuma posição)
- Funciona com touch e mouse
- Tema escuro

---

## 🔍 Mistérios em Série — `misterios.html`

Jogo de dedução lógica com progressão infinita e dificuldade crescente.

### Temas disponíveis

| # | Tema | Suspeitos | Locais | Pistas |
|---|------|-----------|--------|--------|
| 1 | 🎂 O Bolo | Irmão, Cachorro, Prima, Tio | Cozinha, Sala, Quintal, Varanda | Pegada, Farelo, Pelo, Guardanapo |
| 2 | 🏫 A Escola | Zelador, Diretor, Aluno, Professora | Diretoria, Laboratório, Quadra, Biblioteca | Óculos, Bilhete, Chaveiro, Caneta |
| 3 | 🎡 O Parque | Palhaço, Mágico, Pipoqueiro, Guarda | Carrossel, Roda-Gigante, Circo, Lago | Balão, Ingresso, Pipoca, Cartola |
| 4 | 🐾 Pet Shop | Gato, Furão, Papagaio, Hamster | Gaiola, Banho, Vitrine, Estoque | Ração, Brinquedo, Pena, Coleira |
| 5 | ⛺ Acampamento | Monitor, Instrutor, Guia, Colega | Barraca, Fogueira, Trilha, Rio | Lanterna, Bússola, Mapa, Cantil |

### Mecânica de jogo
- O jogo sorteia secretamente 1 suspeito + 1 local + 1 pista
- O jogador seleciona sua hipótese e confirma o palpite
- **Palpite errado:** perde 1 tentativa e recebe uma eliminação (ex: "Cachorro não é o suspeito")
- **Palpite certo:** avança para a próxima fase

### Progressão infinita e ciclos

| Ciclo | Tentativas | Pistas grátis | Cronômetro | Itens extras (decoy) |
|-------|-----------|--------------|------------|----------------------|
| 1 | 6 | 2 | ❌ | ❌ |
| 2 | 5 | 1 | ❌ | ❌ |
| 3 | 4 | 0 | ✅ (palpite errado = -20s) | ❌ |
| 4+ | 4 | 0 | ✅ | ✅ (1 suspeito/local/pista falso extra) |

- Ao completar os 5 temas, o ciclo aumenta e reinicia do Tema 1 com maior dificuldade
- Loop infinito — nunca acaba

### Interface
- Modo claro (alta legibilidade)
- Seleção por botões (toque para escolher suspeito / local / pista)
- Itens eliminados ficam riscados e inativos
- Overlay de vitória e derrota com pontuação e revelação do segredo
- Banner animado ao entrar num novo ciclo

---

## 🖼️ Foto → Emoji — `foto-emoji.html`

Ferramenta que converte fotos em mosaico de emojis ou miniatura pixelizada.  
Branding **Detilli Hub** · modo escuro/claro · 100% offline.

---

### 🌙☀️ Temas

| Tema | Ação |
|------|------|
| ☀️ Claro | Fundo branco/cinza, textos escuros |
| 🌙 Escuro | Fundo escuro com gradientes (padrão) |
| 💻 Sistema | Detecta automaticamente o tema do celular |

Preferência salva no navegador (`localStorage`).

---

### 📥 Formas de carregar imagem

| Método | Como usar |
|--------|-----------|
| 📁 Enviar arquivo | Clique e selecione JPG/PNG/WEBP |
| 📋 Colar | Cole com Ctrl+V ou botão "Colar" |
| URL | Cole o endereço da imagem e clique em Carregar |
| Arrastar | Arraste e solte a imagem no preview |

---

### 🎭 Modo Emoji

Converte a foto em mosaico de emojis coloridos.

#### Miniaturização
- **Slider "Colunas de emoji"** (20–140): controla quantas colunas de emojis formam o mosaico
  - Menos colunas = emojis maiores, mais abstrato
  - Mais colunas = mais emojis, mais detalhe
- **Atalhos rápidos:** Baixo (35) · Médio (60) · Alto (90) · Extremo (130)
- **Slider "Tamanho do emoji (px)"** (10–36): controla o tamanho físico de cada emoji no canvas de saída

#### Paletas de Emoji

| Paleta | Emojis |
|--------|--------|
| Clássico | 😀 ❤️ ⭐ 🎮 📻 🔥 💧 🌙 ☀️ 🍀 🍕 🎈 |
| Rostos | 😀 😁 😂 😍 😎 🥳 😢 😡 🤔 😴 😱 🥰 |
| Natureza | 🌳 🌸 ☀️ 🌊 🍂 ⛰️ 🌵 🌈 ❄️ 🍁 🌻 🌴 |
| Comida | 🍎 🍌 🍇 🥑 🍕 🍫 🍉 🍓 🥕 🍩 🍊 🍋 |
| Animais | 🐶 🐱 🦊 🐼 🐸 🐵 🦁 🐨 🐷 🐧 🐢 🦋 |
| Blocos de cor | 🟥 🟧 🟨 🟩 🟦 🟪 ⬛ ⬜ 🟫 🔴 🟡 🟢 |

- Toque em cada emoji para ativar/desativar
- **Botão Todos / Nenhum** para seleção rápida
- **Campo personalizado:** cole qualquer emoji e clique "+ Add" para adicionar à paleta

#### Algoritmo de cor (alta fidelidade)
- Cada emoji tem sua cor real **calculada automaticamente** (renderiza o emoji em canvas e mede a cor média dos pixels com ponderação por alpha)
- Distância perceptual ponderada: peso 30% vermelho · 59% verde · 11% azul (imita a sensibilidade do olho humano)
- Resultado: mosaico muito mais fiel à foto original do que com cores hardcoded

---

### 🖼️ Modo Miniatura Fiel (módulo separado)

Reduz a foto a uma miniatura real em pixels — sem emojis, apenas pixels originais.

#### Slider de Redução (5% – 100%)

| Posição | Largura de saída | Descrição |
|---------|-----------------|-----------|
| 5% (Micro) | ~10 px | Mínimo — quase imperceptível |
| 20% | ~40 px | 20% do tamanho "polegar" |
| 50% | ~100 px | Metade do polegar |
| 100% (Polegar) | ~200 px | Miniatura "polegar" completa |

- **Atalhos rápidos:** Micro (5%) · 20% polegar · 50% · Polegar (100%)
- O canvas é exibido **ampliado na tela** para visualização, mas exportado no tamanho real mínimo

#### Modos de renderização

| Modo | Resultado |
|------|-----------|
| 🔵 Suave | Interpolação bicúbica — miniatura limpa e fiel (como foto real pequena) |
| 🟣 Pixelizado | Cada pixel vira um bloco visível — efeito retrô/artístico |

- Toggle **"Exibir ampliada"**: mostra a miniatura escalonada na tela para facilitar visualização do detalhe

---

### 🎨 Ajustes de Imagem (compartilhado entre modos)

| Controle | Faixa | Efeito |
|----------|-------|--------|
| Brilho | 40% – 180% | Clareia ou escurece |
| Contraste | 40% – 200% | Aumenta ou reduz diferença entre tons |
| Saturação | 0% – 200% | 0% = preto e branco total, 200% = cores vibrantes |
| Filtro | Normal / P&B / Sépia / Negativo | Aplica efeito global |
| Fundo | Transparente / Preto / Branco / Cor personalizada | Cor de fundo do canvas exportado |

Todos os ajustes são aplicados via `CanvasRenderingContext2D.filter` antes da conversão.

#### Atualização automática
- Toggle **"Atualizar automaticamente"**: recalcula o mosaico com 220ms de debounce a cada mudança de slider (desligável para economizar performance)

---

### 📤 Compartilhar

Ao clicar em **📤 Compartilhar**, abre painel com prévia da imagem e opções:

| Opção | Disponibilidade | O que faz |
|-------|----------------|-----------|
| 📱 Aplicativos | Android/iOS com Web Share API | Abre menu nativo do celular (WhatsApp, Instagram, etc.) |
| 💬 WhatsApp | Sempre | Abre WhatsApp Web com mensagem + link do app |
| 📋 Copiar imagem | Browsers modernos | Copia imagem para área de transferência |
| ⬇️ Baixar PNG | Sempre | Baixa o arquivo PNG |
| 🔵 Enviar ao OIO | Somente quando embutido no OIO | Envia imagem via `postMessage` para o app pai |

---

### 💾 Exportação

| Botão | Formato | Observação |
|-------|---------|------------|
| ⬇️ PNG | PNG com transparência | Preserva fundo transparente se selecionado |
| ⬇️ JPG | JPEG 92% de qualidade | Fundo branco automático se fundo era transparente |
| 📋 Copiar | PNG no clipboard | Ctrl+V em qualquer app para colar |

---

### 🔗 Integração com OIO (`postMessage`)

Quando a ferramenta está embutida como `<iframe>` no OIO (`oio-fam.lovable.app`), o botão **🔵 Enviar ao OIO** envia a imagem gerada para o app pai:

```js
// Mensagem enviada pelo Foto → Emoji para o OIO
{
  type: "detilli-hub-share",
  action: "share-image",
  imageDataUrl: "data:image/png;base64,...",  // imagem PNG completa em base64
  title: "Foto em Emoji 🎨",
  source: "foto-emoji"
}
```

**Código para o OIO escutar:**
```js
window.addEventListener('message', (event) => {
  if (event.origin !== 'https://detiillimichel-max.github.io') return;
  if (event.data?.type === 'detilli-hub-share') {
    const imagem = event.data.imageDataUrl; // PNG base64 — usar aqui
    const titulo = event.data.title;
  }
});
```

**Como embutir no OIO:**
```html
<iframe
  src="https://detiillimichel-max.github.io/emojs-foto/"
  allow="clipboard-write; web-share"
  style="width:100%; height:100%; border:none;">
</iframe>
```

---

## 🚀 Deploy — GitHub Pages

### Estrutura no repositório
```
📁 repositório/
├── index.html        ← Hub central (hub.txt renomeado)
├── futebol.html      ← World Penalty Champion
├── cilada.html       ← CILADA! puzzle
├── misterios.html    ← Mistérios em Série
└── foto-emoji.html   ← Foto → Emoji
```

### Passo a passo
1. No repositório GitHub, clique em **Add file → Upload files**
2. Faça upload de todos os arquivos `.html` de uma vez
3. Em **Settings → Pages**, selecione a branch `main` e pasta `/root`
4. O site estará disponível em `https://seu-usuario.github.io/seu-repositorio/`

---

## 🛠️ Tecnologias

- **HTML5** + **CSS3** + **JavaScript** puro — sem frameworks, sem build
- **Canvas API** — renderização de emojis e miniaturas
- **Web Share API** — compartilhamento nativo mobile
- **Clipboard API** — copiar imagem para área de transferência
- **localStorage** — persistência de preferência de tema
- **Intl.Segmenter** — parse correto de emojis compostos (ZWJ sequences)
- **postMessage API** — comunicação entre iframes (integração OIO)
- **CSS Custom Properties** — sistema de temas claro/escuro

---

*Feito com ♥ no Detilli Hub — tudo roda no navegador, sem servidores, sem cadastro.*
