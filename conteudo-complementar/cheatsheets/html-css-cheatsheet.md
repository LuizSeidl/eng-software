# 📋 HTML & CSS Cheatsheet

## HTML — Estrutura básica
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
  </body>
</html>

## HTML — Tags principais
<h1> a <h6>        # títulos
<p>                # parágrafo
<a href="#">       # link
<img src="" alt=""> # imagem
<ul> <ol> <li>     # listas
<div>              # bloco genérico
<span>             # inline genérico
<form>             # formulário
<input type="">    # campo de entrada
<button>           # botão
<table>            # tabela

## HTML5 — Tags Semânticas
<header>              # cabeçalho da página ou seção
<nav>                 # menu principal de navegação
<main>                # conteúdo principal e exclusivo da página
<section>             # agrupamento temático de conteúdo
<article>             # conteúdo independente e autocontido
<footer>              # rodapé da página ou seção

## CSS — Seletores
elemento           # tag
.classe            # classe
#id                # id
elemento:hover     # pseudo-classe
elemento::before   # pseudo-elemento

## CSS — Box Model
margin             # espaço externo
padding            # espaço interno
border             # borda
width / height     # tamanho

## CSS — Flexbox
display: flex;
justify-content: center;
align-items: center;
flex-direction: row;
gap: 10px;

## CSS — Grid
display: grid;
grid-template-columns: 1fr 1fr;
grid-gap: 10px;

## CSS — Responsividade
@media (max-width: 768px) {
  /* mobile */
}
