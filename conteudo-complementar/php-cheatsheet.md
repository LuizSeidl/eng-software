# 📋 PHP Cheatsheet

## Sintaxe básica
<?php
  echo "Olá Mundo";
?>

## Variáveis
$nome = "João";
$idade = 20;
$preco = 9.99;
$ativo = true;

## Strings
strlen($s)
strtoupper($s)
strtolower($s)
str_replace("a", "b", $s)
explode(",", $s)      # divide em array
implode(",", $arr)    # une array

## Arrays
$arr = [1, 2, 3];
$arr[] = 4;           # adiciona
count($arr)           # tamanho
array_push($arr, 5)
array_pop($arr)
sort($arr)

## Arrays associativos
$pessoa = ["nome" => "João", "idade" => 20];
$pessoa["nome"]

## Controle de fluxo
if ($x > 0) {}
elseif ($x == 0) {}
else {}

for ($i = 0; $i < 10; $i++) {}
foreach ($arr as $val) {}
foreach ($arr as $chave => $val) {}
while ($x > 0) {}

## Funções
function soma($a, $b) {
  return $a + $b;
}

## Superglobais
$_GET["param"]
$_POST["campo"]
$_SESSION["usuario"]
$_COOKIE["token"]

## Conexão MySQL (PDO)
$pdo = new PDO("mysql:host=localhost;dbname=db", "user", "pass");
$stmt = $pdo->prepare("SELECT * FROM tabela WHERE id = ?");
$stmt->execute([$id]);
$dados = $stmt->fetchAll();
