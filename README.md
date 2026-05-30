# 🚀 Guia Prático de CSS Flexbox

<p align="center">
  <span style="color: #2f81f7;"><b>Um guia definitivo e de referência rápida para dominar layouts flexíveis, fluidos e responsivos.</b></span>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/CSS3-Modern_Layout-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Status-Completo_%26_Prático-success?style=for-the-badge" alt="Status" />
  <img src="https://img.shields.io/badge/Nível-Básico_ao_Avançado-7B61FF?style=for-the-badge" alt="Nível" />
</p>

---

## 📖 O que é o Flexbox?

O **Flexible Box Layout (Flexbox)** é um modelo de layout unidimensional do CSS3 feito para distribuir o espaço entre os itens de uma interface e melhorar suas capacidades de alinhamento, seja horizontalmente ou verticalmente. 

Diferente dos modelos tradicionais (`block`, `inline`), o Flexbox foi desenhado para **mudar a largura e a altura dos itens dinamicamente** para preencher o espaço disponível da melhor forma possível, evitando quebras de layout em telas de diferentes tamanhos (responsividade natural).

---

## 🧭 Os Dois Eixos Fundamentais

Para dominar o Flexbox, você precisa entender que ele trabalha com base em dois eixos cartesianos modulares. Quem dita a direção deles é a propriedade `flex-direction`:

1. <span style="color: #2f81f7;"><b>Main Axis (Eixo Principal):</b></span> É o eixo primário ao longo do qual os itens flexíveis são dispostos.
2. <span style="color: #2f81f7;"><b>Cross Axis (Eixo Cruzado):</b></span> É o eixo perpendicular ao eixo principal.

---

## 🛠️ Guia de Propriedades (Cheat Sheet)

### 🔲 1. Propriedades para o Contêiner Pai (`flex-container`)

Para ativar o contexto flexível, aplicamos `display: flex;` ou `display: inline-flex;` no elemento pai.

#### 🔄 Direção e Quebra (`flex-direction` & `flex-wrap`)
* `flex-direction`: Define para onde o Eixo Principal aponta.
  * `row` (padrão): Itens da esquerda para a direita.
  * `row-reverse`: Itens da direita para a esquerda.
  * `column`: Itens de cima para baixo.
  * `column-reverse`: Itens de baixo para cima.
* `flex-wrap`: Define se os itens devem quebrar linha caso falte espaço.
  * `nowrap` (padrão): Força todos os itens na mesma linha (pode gerar transbordo).
  * `wrap`: Quebra os itens para a próxima linha quando necessário.

#### ↔️ Alinhamento no Eixo Principal (`justify-content`)
Controla como o espaço restante é distribuído ao longo do **Main Axis**:
* `flex-start` (padrão): Itens alinhados no início do contêiner.
* `center`: Itens centralizados.
* `flex-end`: Itens alinhados no final do contêiner.
* `space-between`: O primeiro item fica no início, o último no fim, e o espaço é distribuído igualmente entre os do meio.
* `space-around`: Distribui o espaço igualmente ao redor de cada item (as bordas externas têm metade do espaço interno).
* `space-evenly`: Todos os espaços (entre itens e até as bordas) são rigorosamente iguais.

#### ↕️ Alinhamento no Eixo Cruzado (`align-items` & `align-content`)
Controla o alinhamento ao longo do **Cross Axis**:
* `align-items` (Para contêineres de **linha única**):
  * `stretch` (padrão): Estica os itens para preencher todo o eixo cruzado.
  * `flex-start`: Alinha os itens no topo/início do eixo cruzado.
  * `center`: Centraliza verticalmente os itens.
  * `flex-end`: Alinha os itens na base/fim do eixo cruzado.
  * `baseline`: Alinha os itens com base na linha de base dos seus textos internos.
* `align-content` (Apenas para contêineres de **múltiplas linhas** - `wrap` ativo):
  * Modifica o alinhamento das linhas inteiras da mesma forma que o `justify-content` faz com os itens individuais.

---

### 🔹 2. Propriedades para os Itens Filhos (`flex-items`)

Aplicadas diretamente nos elementos que estão dentro do contêiner flexível:

* `order`: Altera a ordem de exibição dos itens sem mexer no HTML (aceita números inteiros negativos e positivos).
* `flex-grow`: Define a habilidade de um item crescer para ocupar o espaço disponível caso necessário (aceita valores proporcionais como `1`, `2`, etc.).
* `flex-shrink`: Define a capacidade de um item diminuir caso o contêiner aperte (padrão é `1`).
* `flex-basis`: Define o tamanho padrão inicial de um elemento antes do espaço restante ser distribuído (substitui o `width`/`height` dentro do fluxo flex).
* `align-self`: Permite que um único item filho ignore a regra geral do `align-items` do pai e tenha um alinhamento exclusivo para si no eixo cruzado.

---

## 📌 Estrutura dos Exemplos do Repositório

Neste laboratório de testes práticos, os arquivos estão organizados para demonstrar visualmente cada cenário acima:

```text
├── index.html          # Estrutura de visualização e painel de testes
├── style.css           # Implementação pura de CSS estruturado em blocos comentados
└── README.md           # Documentação do projeto
```
## ⚖️ Licença

Este projeto está sob a licença **MIT**. Para mais detalhes, consulte o arquivo [LICENSE](LICENSE) incluído neste repositório.
