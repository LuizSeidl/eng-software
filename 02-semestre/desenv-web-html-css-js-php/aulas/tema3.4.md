# 📝 HTML — Formulários

Guia técnico completo sobre construção, organização e validação de formulários HTML5 para coleta de dados com acessibilidade e interatividade.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Nível](https://img.shields.io/badge/Nível-Intermediário-orange)
![W3C](https://img.shields.io/badge/Padrão-W3C-green)

---

## 🏗️ Estrutura Fundamental

```html
<form action="/enviar" method="POST">
  <fieldset>
    <legend>Dados Pessoais</legend>

    <label for="nome">Nome</label>
    <input type="text" id="nome" name="nome" required />

    <label for="email">E-mail</label>
    <input type="email" id="email" name="email" required />
  </fieldset>

  <button type="submit">Enviar</button>
  <button type="reset">Limpar</button>
</form>
```

### Tags estruturais

| Tag          | Função                                                          |
| ------------ | --------------------------------------------------------------- |
| `<form>`     | Container principal — agrupa todos os campos                    |
| `<fieldset>` | Agrupa campos em seções lógicas                                 |
| `<legend>`   | Título descritivo de um `<fieldset>`                            |
| `<label>`    | Legenda do campo — ativa o campo ao clicar (via atributo `for`) |

### Atributos do `<form>`

| Atributo     | Função                                                   |
| ------------ | -------------------------------------------------------- |
| `action`     | URL de destino dos dados ao enviar                       |
| `method`     | Método HTTP: `GET` (URL) ou `POST` (corpo da requisição) |
| `novalidate` | Desativa a validação nativa do navegador                 |

---

## 🎛️ Elementos de Entrada

```html
<!-- Campo de texto simples -->
<input type="text" placeholder="Digite seu nome" />

<!-- Múltiplas linhas -->
<textarea rows="4" cols="40">Texto inicial...</textarea>

<!-- Lista de seleção -->
<select name="cidade">
  <option value="sp">São Paulo</option>
  <option value="rj">Rio de Janeiro</option>
</select>

<!-- Botões -->
<button type="submit">Enviar</button>
<button type="reset">Limpar</button>
```

---

## 🔣 Tipos de `<input>`

| `type`     | Comportamento / Uso                         |
| ---------- | ------------------------------------------- |
| `text`     | Campo de texto genérico                     |
| `email`    | Valida formato com `@` e domínio            |
| `tel`      | Campo para números de telefone              |
| `number`   | Componente numérico com setas de incremento |
| `date`     | Seletor de data via calendário nativo       |
| `datetime` | Seletor de data e horário                   |
| `password` | Oculta os caracteres digitados              |
| `checkbox` | Caixa de seleção múltipla                   |
| `radio`    | Seleção única entre opções de um grupo      |
| `file`     | Upload de arquivos                          |
| `hidden`   | Campo invisível para dados internos         |

---

## ⚙️ Atributos de Controle

| Atributo      | Efeito                                                |
| ------------- | ----------------------------------------------------- |
| `placeholder` | Texto de dica exibido dentro do campo vazio           |
| `autofocus`   | Foca o campo automaticamente ao carregar a página     |
| `minlength`   | Quantidade mínima de caracteres permitida             |
| `maxlength`   | Quantidade máxima de caracteres permitida             |
| `min` / `max` | Valor mínimo e máximo para campos numéricos e de data |
| `disabled`    | Desativa o campo — não é enviado com o formulário     |
| `readonly`    | Campo visível, porém não editável                     |

---

## ✅ Validação Nativa (HTML5)

O HTML5 permite validar dados **no cliente**, sem JavaScript, antes de enviar ao servidor.

```html
<!-- Obrigatório -->
<input type="text" required />

<!-- Tipagem automática -->
<input type="email" />
<!-- valida formato de e-mail -->
<input type="number" />
<!-- aceita apenas números    -->

<!-- Padrão com RegEx -->
<input type="text" pattern="\d{3}\.\d{3}\.\d{3}-\d{2}" placeholder="CPF" />
```

### Tipos de validação

| Tipo            | Atributo / Recurso        | Descrição                                         |
| --------------- | ------------------------- | ------------------------------------------------- |
| Obrigatoriedade | `required`                | Impede envio se o campo estiver vazio             |
| Tipagem         | `type`                    | Verifica consistência com o tipo definido         |
| Padrão (RegEx)  | `pattern`                 | Valida contra uma expressão regular personalizada |
| Comprimento     | `minlength` / `maxlength` | Limita o número de caracteres                     |

> 💡 Para desativar a validação nativa (ex: ao implementar validação customizada via JS), adicione `novalidate` à tag `<form>`.

---

## 💡 Boas Práticas

- Sempre associe `<label>` aos campos via atributo `for` — essencial para acessibilidade
- Use `<fieldset>` e `<legend>` para agrupar campos relacionados logicamente
- Prefira `method="POST"` para dados sensíveis — `GET` expõe os dados na URL
- Utilize os tipos de `<input>` corretos para ativar teclados apropriados em dispositivos móveis
- Combine validação nativa (HTML5) com validação no servidor — nunca confie apenas no cliente

---

_Baseado nos padrões HTML5 — W3C Living Standard_
