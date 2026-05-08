# 🗂️ HTML — Listas, Tabelas e Mídias

Guia técnico sobre estruturação de dados complexos e integração de elementos multimídia em HTML5 de forma moderna e acessível.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Nível](https://img.shields.io/badge/Nível-Intermediário-orange)
![W3C](https://img.shields.io/badge/Padrão-W3C-green)

---

## 📋 Tipos de Listas

| Tipo         | Container | Item   | Descrição | Quando usar                         |
| ------------ | --------- | ------ | --------- | ----------------------------------- |
| Ordenada     | `<ol>`    | `<li>` | —         | Sequência importa (passos, ranking) |
| Não ordenada | `<ul>`    | `<li>` | —         | Itens sem ordem específica          |
| De definição | `<dl>`    | `<dt>` | `<dd>`    | Termos com suas descrições          |

```html
<!-- Ordenada -->
<ol>
  <li>Primeiro passo</li>
  <li>Segundo passo</li>
</ol>

<!-- Não ordenada -->
<ul>
  <li>Item A</li>
  <li>Item B</li>
</ul>

<!-- Definição -->
<dl>
  <dt>HTML</dt>
  <dd>Linguagem de marcação para estruturar páginas web</dd>
</dl>
```

> Listas podem ser **aninhadas** (uma dentro da outra). Marcadores e numeração são customizáveis via CSS.

---

## 📊 Tabelas

### Estrutura básica

```html
<table>
  <thead>
    <tr>
      <th>Nome</th>
      <th>Idade</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Ana</td>
      <td>28</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Total: 1 registro</td>
    </tr>
  </tfoot>
</table>
```

### Tags e atributos

| Tag / Atributo | Função                                          |
| -------------- | ----------------------------------------------- |
| `<table>`      | Container principal da tabela                   |
| `<tr>`         | Define uma linha                                |
| `<td>`         | Célula de dado — deve estar dentro de `<tr>`    |
| `<th>`         | Célula de cabeçalho — valor semântico e visual  |
| `<thead>`      | Agrupa as linhas de cabeçalho                   |
| `<tfoot>`      | Agrupa as linhas de rodapé                      |
| `colspan="N"`  | Expande a célula por **N colunas** (horizontal) |
| `rowspan="N"`  | Expande a célula por **N linhas** (vertical)    |

### Mesclagem de células

```html
<tr>
  <td colspan="2">Ocupa 2 colunas →</td>
</tr>
<tr>
  <td rowspan="2">Ocupa 2 linhas ↓</td>
  <td>Normal</td>
</tr>
```

> ⚠️ **Evite** usar tabelas para layout de página. Essa prática prejudica acessibilidade e é considerada obsoleta — use CSS (Flexbox / Grid) para estruturar o layout.

---

## 🎬 Mídias — Vídeo e Áudio

Com o HTML5, multimídia é nativa — sem necessidade de plugins externos.

```html
<!-- Vídeo -->
<video src="video.mp4" controls autoplay loop>Seu navegador não suporta o elemento de vídeo.</video>

<!-- Áudio -->
<audio src="audio.mp3" controls loop>Seu navegador não suporta o elemento de áudio.</audio>
```

### Atributos principais

| Atributo   | Efeito                                              |
| ---------- | --------------------------------------------------- |
| `src`      | Caminho ou URL do arquivo de mídia                  |
| `controls` | Exibe interface nativa (play, pause, volume)        |
| `autoplay` | Inicia a mídia automaticamente ao carregar a página |
| `loop`     | Reinicia automaticamente ao chegar no final         |

> 💡 Além dos atributos, o HTML5 expõe **Media Events** que permitem controlar vídeo e áudio via JavaScript para interações avançadas (ex: `play`, `pause`, `timeupdate`, `ended`).

---

## 💡 Boas Práticas

- Use `<thead>`, `<tbody>` e `<tfoot>` para tabelas semânticas e acessíveis
- Prefira `<th>` para cabeçalhos — leitores de tela os interpretam corretamente
- Nunca use `<table>` para layout de página — use CSS moderno
- Sempre inclua texto alternativo dentro de `<video>` e `<audio>` para navegadores sem suporte
- Controle estilos de listas (marcadores, numeração) exclusivamente via CSS

---

_Baseado nos padrões HTML5 — W3C Living Standard_
