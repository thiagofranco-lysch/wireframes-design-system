# Design System — Swiss/Editorial

Baseado em referências do estilo tipográfico internacional (Swiss Style).
Aplicar estes tokens e princípios em todos os wireframes e componentes do projeto.

---

## Paleta de cores

| Token         | Hex       | Uso                                          |
|---------------|-----------|----------------------------------------------|
| `color-black` | `#111111` | Texto principal, fundos escuros              |
| `color-white` | `#FFFFFF` | Fundo padrão, texto sobre escuro             |
| `color-off-white` | `#F2F2F0` | Superfícies secundárias, fundos de seção |
| `color-accent` | `#FF3B1F` | Subtítulos destacados, elementos de ênfase  |
| `color-border` | `rgba(0,0,0,0.12)` | Divisores e bordas estruturais      |

**Regras:**
- A paleta é essencialmente monocromática. Preto, branco e off-white respondem por ~95% da composição.
- O acento (`#FF3B1F`) é usado com parcimônia — subtítulos, um traço curto, um label. Nunca como cor de fundo.
- Sem gradientes, sombras ou efeitos decorativos.

---

## Tipografia

A fonte deve ser uma grotesca sem serifa com variação de peso — ex: Helvetica Neue, Inter, ou similar.

| Nível     | Tamanho | Peso | Tracking       | Uso                              |
|-----------|---------|------|----------------|----------------------------------|
| Display   | 48–96px | 700  | –0.02em        | Títulos de capa, números grandes |
| Heading 1 | 32px    | 700  | –0.01em        | Títulos de seção                 |
| Heading 2 | 20px    | 500  | 0              | Subtítulos                       |
| Body      | 14–16px | 400  | 0              | Corpo de texto, linha-altura 1.6 |
| Label     | 11px    | 500  | +0.07em / uppercase | Rótulos, metadados, cabeçalhos de tabela |

**Regras:**
- Hierarquia é construída por tamanho e peso — nunca por cor (exceto o acento pontual).
- Labels sempre em uppercase com tracking positivo.
- Sem itálico decorativo. Sem sublinhado fora de links.
- Contraste de peso é intencional: display bold pesado convive com body regular fino.

---

## Espaçamento

Escala base **4px**. Todos os valores de margin, padding e gap devem ser múltiplos de 4.

| Token      | Valor |
|------------|-------|
| `space-1`  | 4px   |
| `space-2`  | 8px   |
| `space-4`  | 16px  |
| `space-6`  | 24px  |
| `space-8`  | 32px  |
| `space-12` | 48px  |
| `space-16` | 64px  |
| `space-20` | 80px  |

**Regras:**
- O espaço em branco é um elemento de design — não é ausência de conteúdo.
- Seções distintas recebem separação generosa (`space-12` ou `space-16`).
- Nunca comprimir conteúdo para "aproveitar" espaço disponível.

---

## Grid

- **Colunas:** 12
- **Gutter:** 24px
- **Margem lateral:** 40–64px (varia por formato)
- **Largura máxima de conteúdo:** ~65–70% da largura total em layouts de leitura (relatórios, artigos)

**Regras:**
- Todo elemento ancora em uma linha de grade.
- Margens externas são constantes — nunca deixar conteúdo "sangrar" para a borda sem intenção.
- Layouts de múltiplas colunas preferem 2 ou 3 colunas; evitar 4+ em documentos.

---

## Bordas e divisores

| Tipo                  | Valor                              | Uso                        |
|-----------------------|------------------------------------|----------------------------|
| Divisor padrão        | `0.5px solid rgba(0,0,0,0.12)`    | Separação entre seções     |
| Borda estrutural      | `1px solid #111111`                | Contorno de componentes    |
| Traço de acento       | `2px solid #FF3B1F` (largura 24px) | Marcador visual de subtítulo |

**Regras:**
- Sem `border-radius` expressivo — cantos retos ou com raio mínimo (`2–4px`).
- Sem box-shadow decorativa.
- Divisores são finos e discretos — estruturam sem chamar atenção.

---

## Princípios de composição

1. **Tipografia como estrutura** — a hierarquia visual emerge do tipo, não de ícones, cores ou ornamentos.
2. **Grid rígido** — consistência de alinhamento cria confiança e leiturabilidade.
3. **Silêncio intencional** — espaço em branco generoso. Conteúdo respira; páginas não competem.
4. **Acento pontual** — o vermelho aparece uma vez por composição, no elemento de maior hierarquia secundária.
5. **Sem decoração sem função** — cada elemento visual justifica sua presença.

---

## Aplicação em wireframes

Ao gerar wireframes com este Design System:

- Usar retângulos sem preenchimento ou com `color-off-white` para containers.
- Representar texto com blocos proporcionais ao nível tipográfico (não lorem ipsum genérico).
- Indicar onde o acento aparece com uma nota ou cor diferenciada no wireframe.
- Manter margens e gutters fiéis à escala de 4px.
- Preferir layouts de 1 ou 2 colunas; 3 colunas apenas quando o conteúdo justificar.
