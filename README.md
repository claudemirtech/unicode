# AtomicWeb - Conversor Unicode

<div align="center">

[![Deploy static content to Pages](https://github.com/claudemirtech/unicode/actions/workflows/static.yml/badge.svg)](https://github.com/claudemirtech/unicode/actions/workflows/static.yml)
[![GitHub Pages](https://img.shields.io/badge/Demo-Disponível%20Online-blue?style=flat&logo=githubpages)](https://atomicweb.com.br/unicode)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)

**Ferramenta prática e rápida para converter caracteres especiais e acentuados na sua representação Unicode escape (`\uXXXX`).**

[🌐 Acessar Demonstração Online](https://atomicweb.com.br/unicode) • [Reportar Problema](https://github.com/claudemirtech/unicode/issues)

</div>

---

## 📌 Sobre o Projeto

O **Conversor Unicode** da AtomicWeb é uma aplicação web leve e responsiva criada para facilitar a vida de desenvolvedores, analistas e administradores de sistemas que precisam converter textos contendo acentos, caracteres especiais ou emojis para sequências de escape Unicode (como `\u00e1`, `\u00e7`, `\u00f5`).

Essas sequências são fundamentais ao trabalhar com formatos como **JSON**, arquivos de propriedades (`.properties`), configurações em YAML/XML, bancos de dados legados ou linguagens como Java, Python, C#, PHP e JavaScript, evitando problemas de encoding (UTF-8 / ISO-8859-1 / ASCII).

---

## 🚀 Funcionalidades

- ⚡ **Conversão Flexível**:
  - **Manter caracteres ASCII (padrão)**: Converte apenas acentuação e caracteres especiais, mantendo o restante legível (ex: `café` ➔ `caf\u00e9`).
  - **Converter todos os caracteres**: Codifica todos os caracteres legíveis para Unicode, preservando espaços e quebras de linha.
- 🔠 **Controle de Caixa (Hexadecimal)**:
  - Opção para gerar códigos com letras maiúsculas (`\u00E1`) ou minúsculas (`\u00e1`).
- 🎯 **Exemplos Rápidos**:
  - Botões de teste com 1 clique (`Usuários`, `café`, `maçã`, `canção`, emojis `😀🎉❤️`).
- 📊 **Informações Detalhadas e Diagnóstico**:
  - Contagem total de caracteres em tempo real.
  - Total de caracteres especiais identificados.
  - Tamanho final do texto convertido.
  - Tabela discriminando cada caractere especial único, seu código padrão (`U+XXXX`) e seu escape (`\uXXXX`).
- 📋 **Cópia Instantânea**:
  - Copie o resultado clicando diretamente na caixa de exibição ou no botão dedicado, com feedback visual instantâneo.
- ⌨️ **Atalho de Teclado**:
  - Pressione `Ctrl + Enter` no campo de texto para acionar a conversão instantaneamente.
- 📱 **Interface Moderna e Responsiva**:
  - Totalmente adaptada para desktops, tablets e smartphones com a identidade visual da **AtomicWeb**.
- 🔒 **100% Client-Side**:
  - Seus dados não saem do navegador; todo o processamento ocorre localmente via JavaScript.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e acessível.
- **Tailwind CSS (CDN)**: Estilização moderna e layout responsivo.
- **JavaScript (ES6+)**: Lógica pura no cliente (Vanilla JS), sem dependência de frameworks ou gerenciadores de pacotes pesados.
- **GitHub Actions & GitHub Pages**: Pipeline de Integração Contínua e Deploy Contínuo (CI/CD) para publicação automática de conteúdo estático.

---

## 📂 Estrutura do Repositório

```text
unicode/
├── .github/
│   └── workflows/
│       └── static.yml       # Fluxo de CI/CD para deploy no GitHub Pages
├── img/
│   ├── favicon.ico          # Favicon da aplicação
│   ├── logo.svg             # Logotipo em formato vetorial
│   └── logo192.png          # Ícone para dispositivos móveis
├── index.html               # Aplicação completa (HTML, CSS Tailwind e JavaScript)
├── README.md                # Documentação do projeto
└── .gitignore               # Configurações de arquivos ignorados pelo Git
```

---

## 💻 Como Executar Localmente

Como a aplicação é estática e não possui dependências de compilação ou backend, rodá-la localmente é muito simples:

### Opção 1: Diretamente no Navegador
Basta clonar o repositório e abrir o arquivo [`index.html`](file:///home/claudemir/Projects/Atomicweb/unicode/index.html) em qualquer navegador web:
```bash
git clone https://github.com/claudemirtech/unicode.git
cd unicode
# No Linux:
xdg-open index.html
# No macOS:
open index.html
# No Windows:
start index.html
```

### Opção 2: Servidor Local Simples

Caso queira usar um servidor HTTP local:

- **Com Python 3:**
  ```bash
  python3 -m http.server 8000
  ```
  Acesse: `http://localhost:8000`

- **Com Node.js (`npx serve`):**
  ```bash
  npx serve .
  ```

- **Com extensão VS Code / IDE:**
  Utilize extensões como **Live Server** para recarregamento automático.

---

## 📖 Exemplo de Uso

| Entrada | Modo "Manter ASCII" | Modo "Todos os Caracteres" |
| :--- | :--- | :--- |
| `café` | `caf\u00e9` | `\u0063\u0061\u0066\u00e9` |
| `Usuários` | `Usu\u00e1rios` | `\u0055\u0073\u0075\u00e1\u0072\u0069\u006f\u0073` |
| `maçã` | `ma\u00e7\u00e3` | `\u006d\u0061\u00e7\u00e3` |

---

## 🤝 Como Contribuir

Contribuições são sempre bem-vindas! Se você tiver sugestões de melhorias ou encontrar algum bug:

1. Faça um Fork do projeto (`fork`).
2. Crie uma Branch para sua Feature ou Correção (`git checkout -b feature/minha-feature`).
3. Faça o Commit de suas alterações (`git commit -m 'feat: adiciona nova funcionalidade'`).
4. Faça o Push para a sua Branch (`git push origin feature/minha-feature`).
5. Abra um **Pull Request**.

---

## 🌐 Autor e Créditos

Desenvolvido por **[AtomicWeb](https://atomicweb.com.br/)** / **Claudemir** ([@claudemirtech](https://github.com/claudemirtech)).

Se este projeto foi útil para você, considere deixar uma ⭐️ no repositório!
