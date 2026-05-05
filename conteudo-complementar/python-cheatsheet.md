# 📋 Python Cheatsheet

## Tipos de dados
x = 10          # int
y = 3.14        # float
s = "texto"     # string
b = True        # bool
l = [1, 2, 3]   # list
t = (1, 2, 3)   # tuple
d = {"a": 1}    # dict
c = {1, 2, 3}   # set

## Strings
s.upper()        # maiúsculas
s.lower()        # minúsculas
s.strip()        # remove espaços
s.split(",")     # divide em lista
s.replace("a","b")
f"Olá {nome}"   # f-string

## Listas
l.append(4)      # adiciona no fim
l.insert(0, 9)   # insere na posição
l.remove(2)      # remove valor
l.pop()          # remove último
l.sort()         # ordena
len(l)           # tamanho

## Dicionários
d["chave"]       # acessa valor
d.get("chave")   # acessa sem erro
d.keys()         # lista chaves
d.values()       # lista valores
d.items()        # pares chave/valor

## Controle de fluxo
if x > 0:
    pass
elif x == 0:
    pass
else:
    pass

for i in range(10):
    pass

while x > 0:
    x -= 1

## Funções
def soma(a, b):
    return a + b

lambda x: x * 2

## Exceções
try:
    pass
except Exception as e:
    print(e)
finally:
    pass

## Arquivos
with open("arquivo.txt", "r") as f:
    conteudo = f.read()
