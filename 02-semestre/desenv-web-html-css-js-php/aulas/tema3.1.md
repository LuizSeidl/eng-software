# 📄 Guia de HTML — Fundamentos

Um guia estruturado sobre a Linguagem de Marcação de Hipertexto, cobrindo conceitos essenciais, evolução histórica e boas práticas para criação de páginas web profissionais.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Nível](https://img.shields.io/badge/Nível-Iniciante-blue)
![W3C](https://img.shields.io/badge/Padrão-W3C-green)

---

## 📌 O que é HTML

HTML não é uma linguagem de programação — é uma **linguagem de marcação** composta por elementos conectados (tags). Seu objetivo é organizar conteúdo e estabelecer a estrutura básica de uma página web, permitindo a inclusão de textos, figuras, tabelas e vídeos de forma hierárquica.

---

## 🕰️ Evolução Histórica

| Ano   | Versão    | Destaque                               |
| ----- | --------- | -------------------------------------- |
| 1991  | HTML 1.0  | Criado por Tim Berners-Lee             |
| 1999  | HTML 4.01 | Padronização consolidada pelo W3C      |
| 2000  | XHTML     | Versão mais rígida, baseada em XML     |
| 2014  | **HTML5** | Suporte a multimídia, semântica e APIs |
| Atual | 5.1 / 5.2 | Correções e novos recursos             |

O HTML nasceu da união dos padrões **SGML** e **HyTime**, sendo mantido e padronizado pelo **W3C** (World Wide Web Consortium).

---

## 🏗️ Estrutura Obrigatória

```html
<!DOCTYPE html>
<html lang="pt">
  <head>
    <meta charset="UTF-8" />
    <title>Título da Página</title>
    <link rel="stylesheet" href="style.css" />
  </head>

  <body>
    <!-- Conteúdo visível aqui -->
  </body>
</html>
```

---

## 🧩 Elementos do `<head>`

| Tag        | Função                                              |
| ---------- | --------------------------------------------------- |
| `<title>`  | Título exibido na aba do navegador                  |
| `<meta>`   | Metainformações: charset, descrição, palavras-chave |
| `<link>`   | Vincula CSS externos e favicons                     |
| `<style>`  | Estilos CSS internos ao documento                   |
| `<script>` | Scripts JavaScript internos ou externos             |

---

## 📐 Seções Comuns de uma Página

- **Cabeçalho** — área superior com título e logomarca
- **Navegação** — links para as seções do site
- **Conteúdo principal** — parte central, pode ter subseções
- **Barra lateral** — informações ou links complementares
- **Rodapé** — copyright, contatos e links informativos

---

## 💡 Boas Práticas

> **Sempre declare o Doctype.** No HTML5, basta `<!DOCTYPE html>` — sem necessidade de DTD externa. Isso garante renderização correta nos navegadores.

> **Salve com a extensão correta.** Use `.html` ou `.htm` em editores como VS Code ou Notepad++.

> **Defina o idioma.** O atributo `lang` na tag `<html>` melhora acessibilidade e SEO.

---

_Baseado nos fundamentos do HTML — W3C Standard_
