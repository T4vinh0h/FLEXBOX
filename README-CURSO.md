# 🎓 Curso HTML & CSS - UC2 Aula 2

## 🌓 Sistema de Temas Claro/Escuro

O curso agora possui um sistema de temas completo com alternância entre modo claro e escuro.

### Como usar:
1. Clique no botão **"🌓 Tema"** no canto superior direito de qualquer página
2. O tema é salvo automaticamente no navegador (localStorage)
3. Ao recarregar a página, o tema escolhido é mantido

### Características dos Temas:

#### 🌞 Tema Claro (Padrão)
- Fundo claro (#f5f5f5)
- Texto escuro (#333333)
- Cores suaves e profissionais
- Ideal para ambientes bem iluminados

#### 🌙 Tema Escuro
- Fundo escuro (#1a1a2e)
- Texto claro (#eaeaea)
- Cores vibrantes com contraste adequado
- Ideal para ambientes com pouca luz ou uso noturno

### Variáveis CSS Personalizadas:
- `--bg-primary`: Cor de fundo principal
- `--bg-secondary`: Cor de fundo secundária
- `--text-primary`: Cor do texto principal
- `--accent-primary`: Cor de destaque principal
- `--accent-secondary`: Cor de destaque secundária
- E muitas outras...

---

## 📱 Responsividade

O curso é totalmente responsivo e se adapta a diferentes tamanhos de tela:

### Desktop (1200px+)
- Layout completo com todas as funcionalidades
- Tabelas com largura total
- Grid de cards com múltiplas colunas

### Tablet (768px - 1199px)
- Grid ajustado automaticamente
- Tabelas com scroll horizontal
- Fontes e espaçamentos proporcionais

### Mobile (até 767px)
- Layout de coluna única
- Tabelas convertidas para formato vertical
- Botões de navegação empilhados
- Toc otimizado para toque

### Tecnologias de Responsividade:
- **CSS Grid**: Para layout de cards
- **Flexbox**: Para navegação e componentes
- **Media Queries**: Para breakpoints específicos
- **Clamp()**: Para fontes responsivas
- **Unidades Relativas**: %, vw, vh, rem

---

## 📊 Novo Layout com Tabelas

O curso foi reorganizado usando tabelas HTML para melhor visualização:

### Vantagens do Layout com Tabelas:
1. **Organização Visual**: Informações estruturadas em linhas e colunas
2. **Comparação Fácil**: Dados lado a lado para comparação
3. **Responsividade**: Tabelas se adaptam a diferentes telas
4. **Acessibilidade**: Melhor navegação com leitores de tela
5. **Profissional**: Aparência mais organizada e estruturada

### Tipos de Tabelas Usadas:

#### 1. **content-table** - Tabela Principal
- Usada para listar informações principais
- Cabeçalho colorido com destaque
- Linhas alternadas para melhor leitura
- Hover effects para interatividade

#### 2. **info-table** - Tabela de Informação
- Usada para explicar conceitos detalhadamente
- Rótulos na coluna esquerda
- Conteúdo na coluna direita
- Ideal para documentação técnica

### Exemplo de Estrutura:

```html
<table class="content-table">
    <thead>
        <tr>
            <th>Coluna 1</th>
            <th>Coluna 2</th>
            <th>Coluna 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Dado 1</td>
            <td>Dado 2</td>
            <td>Dado 3</td>
        </tr>
    </tbody>
</table>
```

---

## 📁 Estrutura de Arquivos

```
FLEXBOX/
├── aulas.html                          # Página principal do curso
├── html/
│   ├── css/
│   │   ├── style.css                 # CSS original
│   │   └── curso-style.css            # NOVO: CSS do curso com temas
│   ├── aula-1-listas.html             # Aula 1 (formato novo)
│   ├── aula-2-css-basico.html         # Aula 2
│   ├── aula-3-propriedades-css.html   # Aula 3
│   ├── aula-4-classes-ids.html         # Aula 4
│   ├── aula-5-box-model.html           # Aula 5
│   ├── aula-6-display-div-span.html   # Aula 6
│   ├── aula-7-position-zindex.html     # Aula 7
│   ├── aula-8-flexbox.html            # Aula 8
│   ├── aula-9-semantic-html.html       # Aula 9
│   ├── aula-10-formularios.html       # Aula 10
│   └── aula-11-git-github.html        # Aula 11
└── README-CURSO.md                     # Este arquivo
```

---

## 🎨 Personalização de Cores

Para personalizar as cores do curso, edite as variáveis CSS em `html/css/curso-style.css`:

### Tema Claro:
```css
:root {
    --accent-primary: #667eea;
    --accent-secondary: #764ba2;
    --bg-primary: #f5f5f5;
    /* ... outras variáveis */
}
```

### Tema Escuro:
```css
[data-theme="dark"] {
    --accent-primary: #e94560;
    --accent-secondary: #ff6b6b;
    --bg-primary: #1a1a2e;
    /* ... outras variáveis */
}
```

---

## 🔧 Funcionalidades Implementadas

### 1. **Toggle de Tema**
- Botão flutuante no canto superior direito
- Alterna entre modo claro e escuro
- Persistência via localStorage

### 2. **Layout Responsivo**
- Adaptação automática a diferentes tamanhos
- Navegação mobile otimizada
- Tabelas responsivas com scroll

### 3. **Organização Visual**
- Uso de tabelas para estruturar conteúdo
- Cards informativos com hover effects
- Divisores de seção estilizados

### 4. **Acessibilidade**
- Cores com contraste adequado
- Navegação por teclado
- Tags semânticas HTML
- Suporte a leitores de tela

### 5. **Sistema de Progresso**
- Barra de progresso visual
- Persistência de aulas concluídas
- Feedback visual de conclusão

---

## 🚀 Como Usar

### Para Alunos:
1. Abra `aulas.html` no navegador
2. Navegue pelas aulas usando a tabela de conteúdo
3. Clique nos links das aulas para acessar o conteúdo
4. Use o toggle de tema conforme sua preferência
5. Aproveite o layout responsivo em qualquer dispositivo

### Para Desenvolvedores:
1. Edite `html/css/curso-style.css` para personalizar
2. Adicione novas aulas seguindo o formato das existentes
3. Use as classes CSS fornecidas para consistência
4. Teste a responsividade em diferentes tamanhos de tela

---

## 📱 Navegação Mobile

Em dispositivos móveis:
- Tabelas se convertem para formato vertical
- Cards de aulas se organizam em uma coluna
- Botões de navegação ficam empilhados
- Menu de tema otimizado para toque

---

## 🎯 Próximas Melhorias Sugeridas

1. **Busca de Conteúdo**: Adicionar campo de busca nas aulas
2. **Favoritos**: Permitir marcar aulas como favoritas
3. **Anotações**: Sistema para anotar aulas
4. **Quiz**: Questionários ao final de cada módulo
5. **Certificado**: Gerar certificado ao completar o curso
6. **Modo Impressão**: Versão otimizada para impressão

---

## 📞 Suporte

Se encontrar algum problema ou tiver sugestões:
1. Verifique se o navegador suporta CSS moderno
2. Limpe o cache do navegador
3. Teste em diferentes navegadores (Chrome, Firefox, Edge)
4. Verifique o console do navegador para erros

---

## 🏆 Conclusão

O curso agora oferece uma experiência moderna, responsiva e personalizável com:
- ✅ Sistema de temas claro/escuro
- ✅ Layout totalmente responsivo
- ✅ Organização visual com tabelas
- ✅ Design profissional e consistente
- ✅ Acessibilidade aprimorada
- ✅ Performance otimizada

Aproveite ao máximo esta nova experiência de aprendizado! 🎓✨