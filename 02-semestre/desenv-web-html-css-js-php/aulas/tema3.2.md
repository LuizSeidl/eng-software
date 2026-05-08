# 🏗️ HTML — Estrutura, Semântica e Boas Práticas

Um guia técnico sobre os pilares do HTML moderno: estruturação de documentos, semântica HTML5 e boas práticas para acessibilidade e SEO.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Nível](https://img.shields.io/badge/Nível-Intermediário-orange)
![W3C](https://img.shields.io/badge/Padrão-W3C-green)

---

## 🔖 Anatomia das Tags

Tags são palavras delimitadas por `<` e `>` que instruem o navegador sobre estrutura e significado do conteúdo.

```html
<!-- Tag com fechamento obrigatório -->
<h1>Título principal</h1>

<!-- Tag com atributos -->
<img src="imagem.jpg" alt="Descrição" id="foto" class="destaque" />
```

### Atributos Globais Essenciais

| Atributo | Uso                                                       |
| -------- | --------------------------------------------------------- |
| `id`     | Identificador **único** no documento                      |
| `class`  | Agrupa múltiplos elementos para estilos ou comportamentos |
| `href`   | Define o destino de hiperlinks                            |
| `src`    | Caminho de recursos externos (imagem, script)             |

---

## 🧠 Semântica — O Coração do HTML5

Semântica é escolher a tag de acordo com o **significado** do conteúdo, não apenas sua aparência. Beneficia leitores de tela, SEO e manutenção.

```html
<header>
  <!-- Cabeçalho da página ou seção     -->
  <nav><!-- Bloco de links de navegação       --></nav>
</header>

<main>
  <!-- Conteúdo principal e único        -->
  <article>
    <!-- Bloco independente (ex: post)     -->
    <section><!-- Grupo de conteúdo relacionado   --></section>
  </article>
  <aside><!-- Conteúdo periférico / barra lateral --></aside>
</main>

<footer><!-- Rodapé da página ou seção         --></footer>
```

---

## 📝 Organização de Texto

### Hierarquia de títulos

```html
<h1>Título principal — use apenas um por página</h1>
<h2>Subtítulo de seção</h2>
<h3>Subtítulo de subseção</h3>
<!-- h4, h5, h6 para níveis mais profundos -->
```

### Elementos de texto

| Tag      | Finalidade                                       |
| -------- | ------------------------------------------------ |
| `<p>`    | Parágrafo de texto comum                         |
| `<div>`  | Contêiner genérico em **bloco**                  |
| `<span>` | Marcação genérica **em linha** (sem quebra)      |
| `<pre>`  | Texto pré-formatado (preserva espaços e quebras) |
| `<br>`   | Quebra de linha                                  |
| `<hr>`   | Linha horizontal de separação temática           |

---

## ✅ Formatação: Visual vs. Semântica

| Tag        | Efeito Visual | Peso Semântico | Recomendado |
| ---------- | ------------- | -------------- | ----------- |
| `<b>`      | Negrito       | ❌ Nenhum      | Evitar      |
| `<strong>` | Negrito       | ✅ Importância | ✅ Sim      |
| `<i>`      | Itálico       | ❌ Nenhum      | Evitar      |
| `<em>`     | Itálico       | ✅ Ênfase      | ✅ Sim      |

> Leitores de tela utilizam `<strong>` e `<em>` para dar entonação diferente ao conteúdo — essencial para acessibilidade.

---

## 🚫 Tags Obsoletas — Evite

Com o HTML5, a responsabilidade visual passou inteiramente ao CSS. As tags abaixo causam problemas em navegadores modernos e devem ser substituídas:

| Tag obsoleta | Substituto moderno            |
| ------------ | ----------------------------- |
| `<center>`   | `text-align: center` (CSS)    |
| `<font>`     | `font-family` / `color` (CSS) |
| `<dir>`      | `<ul>` com CSS                |
| `<applet>`   | `<object>` ou JavaScript      |

---

## 💡 Resumo de Boas Práticas

- Use **um único `<h1>`** por página como título principal
- Prefira tags semânticas (`<article>`, `<section>`) a `<div>` genéricos sempre que possível
- Escolha `<strong>` e `<em>` no lugar de `<b>` e `<i>` para conteúdo com significado
- Mantenha apresentação visual no CSS — nunca em tags HTML obsoletas
- Sempre feche as tags que exigem fechamento

---

_Baseado nos padrões HTML5 — W3C Living Standard_
