# ❤️ O Coração - Experiência Interativa de Aniversário

Uma experiência web imersiva criada para celebrar 2 anos de namoro. Um presente digital que combina memórias, música, mensagens românticas e lugares especiais em uma jornada interativa única.

## 💝 O Que É Isso?

Imagine abrir um presente que nunca é igual duas vezes. Cada vez que você visita, descobre uma nova mensagem romântica, uma foto diferente, uma música que marcou, ou um lugar especial. É como um álbum de memórias vivo que se revela aos poucos.

**Comece com um coração pulsante.** Clique nele e veja o que acontece...

## 🎁 O Que Você Vai Encontrar

### **🔮 Oráculo**
Frases românticas que mudam toda vez que você abre. São 50 mensagens únicas - cada uma falando de um detalhe especial.

### **💌 Carta Especial**
10 cartas diferentes escritas à mão (digitalmente). O texto aparece como se estivesse sendo digitado na hora, em um papel pautado virtual.

### **📸 Memórias**
50 fotos do casal com legendas contando a história de cada momento. Você pode navegar pra frente e pra trás, como se folheasse um álbum físico.

### **🎵 Sinfonias**
50 músicas do Spotify que marcaram o relacionamento, cada uma com uma descrição de por que é especial. Dá pra ouvir direto na página.

### **📍 Mapa**
50 lugares que têm significado especial - restaurantes, praias, a casa onde moraram juntos. Cada foto conta uma história daquele lugar.

### **⏱️ Cronômetro**
Um contador em tempo real mostrando quantos dias já se passaram desde o início do namoro. Atualiza a cada segundo.

### **💬 Mensagens de Boas-Vindas**
100 mensagens únicas que aparecem toda vez que você visita. Nunca repete até completar todas. É como se o site lembrasse de você.

### **🌅 Saudações do Dia**
A página te cumprimenta diferente dependendo da hora: madrugada, manhã, tarde ou noite. São 40 saudações contextuais no total.

## 🚀 Como Usar

1. Abra o arquivo `index.html` no navegador
2. Clique no coração pulsante (aguarde... vai valer a pena)
3. Explore os 5 cards:
   - Clique no **Oráculo** pra ver uma mensagem romântica
   - Abra a **Carta** pra ler uma carta completa
   - Navegue pelas **Memórias** com as flechas nos ornamentos
   - Ouça as **Sinfonias** direto do Spotify
   - Descubra o **Mapa** dos lugares especiais

> **Dica:** Cada modal tem navegação própria - clique nos símbolos `⸸ ✦ ⸸` pra avançar/voltar ou fechar

## 💡 Por Que Criar Isso?

Presentes físicos são legais, mas presentes digitais podem ser infinitos. Em vez de um álbum com 10 fotos, aqui tem 50. Em vez de uma carta, tem 10. Em vez de uma playlist, cada música tem sua própria história.

E o melhor: **nunca é a mesma experiência duas vezes.** Cada visita revela algo novo.

## 🎨 Visual e Atmosfera

O design é **gótico-romântico** - aquele contraste entre escuro e delicado:
- Coração anatômico (vulnerabilidade e realismo)
- Cores vermelhas intensas com sombras brilhantes
- Fonte gótica clássica (Cloister Black)
- Animações suaves que parecem flutuar
- Estilo polaroid nas fotos (nostalgia)

## 📱 Funciona no Celular?

Sim! O layout se adapta automaticamente:
- **Desktop:** Grid com carta central grande
- **Tablet:** 2 colunas
- **Celular:** Tudo empilhado em uma coluna

Todos os botões são grandes o suficiente pra tocar com o dedo.

## 🎭 Detalhes Escondidos (Easter Eggs)

- A mensagem de visita é diferente toda vez (até completar 100)
- As saudações mudam automaticamente a cada 6 horas
- Dá pra fechar os modais clicando nos ornamentos decorativos
- O coração tem 3 estágios de animação antes de explodir

## 📂 Estrutura do Projeto

```
aniversario-namoro/
├── index.html              # Página principal
├── style.css               # Visual e animações
├── script.js               # Mágica acontece aqui
├── CloisterBlack.ttf       # Fonte gótica
├── coracao.png             # Coração principal
├── envelope.png            # Carta selada
├── corrente.png            # Textura de fundo
├── heart.png, fotos.png, musica.png, local.png  # Ícones
├── nos/                    # 50 fotos do casal (1.jpg → 50.jpg)
├── lugares/                # 50 fotos de lugares (1.jpg → 50.jpg)
└── README.md               # Você está aqui
```

## 🔧 Personalizando Para Você

Quer criar algo assim pro seu relacionamento? Veja como:

### **Trocar as Fotos**
1. Substitua os arquivos em `/nos/` e `/lugares/`
2. Edite as descrições no `script.js` (arrays `allPhotos` e `allPlaces`)

### **Mudar as Músicas**
1. Vá no Spotify → Compartilhar → Incorporar playlist
2. Cole o código no array `spotifySongs` dentro do `script.js`

### **Ajustar a Data do Relacionamento**
```javascript
// Linha 9 do script.js
const relationshipStart = new Date('2023-12-04T15:00:00');
```

### **Adicionar Mais Mensagens**
Edite os arrays no `script.js`:
- `oracleMessages` (linha 80): Mensagens do oráculo
- `letters` (linha 130): Cartas completas
- `visitMessages` (linha 200): Mensagens de visita
- `timeGreetings` (linha 40): Saudações por horário

## 💻 Tecnologias Usadas

- **HTML5** - Estrutura da página
- **CSS3** - Visual e animações (20+ animações diferentes!)
- **JavaScript Puro** - Toda a interatividade (sem jQuery, React, nada)
- **Spotify Embed** - Player de música integrado
- **LocalStorage** - Lembra quantas vezes você visitou

## 🎯 Casos de Uso

- 💑 Aniversário de namoro/casamento
- 💝 Presente criativo pra namorado(a)
- 📅 Marcos de relacionamento (6 meses, 1 ano, etc)
- 🎁 Alternativa a cartas físicas
- 📖 Arquivo digital de memórias do casal

---

## 🛠️ Detalhes Técnicos (Pra Quem Curte Código)

<details>
<summary><b>Clique aqui pra ver a parte nerd 🤓</b></summary>

### **Tech Stack Detalhado**
- Vanilla JavaScript ES6+ (500+ linhas)
- CSS Grid + Flexbox para layouts
- CSS Variables para design system
- LocalStorage API para persistência
- Canvas API (não usado, mas planejado)
- Fetch API (não usado, mas disponível)

### **Destaques Técnicos**

#### **1. Efeito Typewriter Inteligente**
```javascript
function typeWriter(element, html, speed = 30)
```
- Mantém formatação HTML enquanto digita
- Suporta parágrafos, quebras de linha, negrito
- Otimizado para mobile (não trava)

#### **2. Sistema de Histórico de Navegação**
```javascript
let galleryHistory = [];
let galleryCurrentIndex = -1;
```
- Cada modal (galeria, mapa, playlist) tem seu próprio histórico
- Navega pra frente/trás sem recarregar
- Adiciona item novo quando chega no final

#### **3. Animações CSS Complexas**
- **Explosão do coração:** `scale(1) → scale(10)` com fade out
- **Float infinito:** Elementos flutuam suavemente pra cima/baixo
- **Pulso sincronizado:** 4 batidas rápidas antes da explosão
- **Vignette cinematográfica:** Escurecimento gradual nas bordas

#### **4. Design System com CSS Variables**
```css
:root {
  --red-primary: #B91818;
  --shadow-glow: 0 0 15px rgba(185, 24, 24, 0.6);
  --transition: 0.3s ease;
  /* 20+ variáveis */
}
```

#### **5. Sistema de Visitas com LocalStorage**
```javascript
let visitCount = parseInt(localStorage.getItem('visitCount')) || 0;
if (visitCount >= 100) visitCount = 0;
visitCount++;
localStorage.setItem('visitCount', visitCount);
```

#### **6. Detecção de Período do Dia**
```javascript
function getTimeOfDay() {
  const hour = new Date().getHours();
  if (hour >= 0 && hour < 6) return 'madrugada';
  if (hour >= 6 && hour < 12) return 'manha';
  if (hour >= 12 && hour < 18) return 'tarde';
  return 'noite';
}
```

### **Decisões de Arquitetura**

**Por que sem framework?**
- Mais leve (sem 100kb+ de biblioteca)
- Mais rápido (sem virtual DOM)
- Mais didático (JavaScript puro)
- Hospedagem grátis simples (GitHub Pages)

**Por que conteúdo aleatório?**
- Incentiva visitas repetidas
- Cada experiência é única
- 50×10×100 = 50.000 combinações possíveis

**Por que localStorage em vez de backend?**
- Simplicidade: sem servidor, sem banco
- Privacidade: tudo fica no seu navegador
- Performance: instantâneo
- Custo: zero hospedagem

### **Performance**

- ✅ Zero dependências externas (exceto Spotify)
- ✅ Fonte customizada com `font-display: swap`
- ✅ Animações com `transform` e `opacity` (GPU-accelerated)
- ✅ Lazy loading implícito em imagens
- ✅ Modals fora do fluxo normal (position: fixed)

### **Acessibilidade**

- ✅ Roles ARIA (`role="dialog"`, `role="button"`)
- ✅ `aria-live="polite"` para contadores dinâmicos
- ✅ `tabindex` para navegação por teclado
- ✅ `aria-label` descritivos em interações
- ✅ `prefers-reduced-motion` para desabilitar animações

### **Estrutura do Código**

```javascript
// script.js (~500 linhas)
├── Constantes (data do relacionamento, arrays de conteúdo)
├── Funções de tempo (countdown, cronômetro, saudações)
├── Sistema de visitas (localStorage)
├── Efeitos visuais (typewriter, explosão do coração)
├── Navegação (histórico de modals)
├── Event listeners (cliques, teclado)
└── Inicialização
```

### **CSS Modular**

```css
/* style.css (~600 linhas) */
├── Variáveis CSS (design system)
├── Reset e base styles
├── Página inicial (coração e countdown)
├── Página principal (grid e cards)
├── Modals (carta, oráculo, galeria)
├── Animações (@keyframes)
├── Responsividade (@media queries)
└── Acessibilidade (prefers-reduced-motion)
```

</details>

---

## 📧 Contato

- **GitHub:** [@enrique-ss](https://github.com/enrique-ss)
- **Email:** enriqueabyss@gmail.com