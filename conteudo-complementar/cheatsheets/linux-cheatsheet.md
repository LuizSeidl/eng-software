# 📋 Linux Cheatsheet

## Navegação
pwd                   # pasta atual
ls                    # lista arquivos
ls -la                # lista com detalhes e ocultos
cd <pasta>            # entra na pasta
cd ..                 # volta um nível
cd ~                  # vai para home

## Arquivos e pastas
touch <arquivo>       # cria arquivo
mkdir <pasta>         # cria pasta
mkdir -p a/b/c        # cria pastas aninhadas
cp <origem> <destino> # copia arquivo
mv <origem> <destino> # move ou renomeia
rm <arquivo>          # remove arquivo
rm -rf <pasta>        # remove pasta e conteúdo

## Visualizar conteúdo
cat <arquivo>         # exibe conteúdo
less <arquivo>        # exibe com scroll
head <arquivo>        # primeiras 10 linhas
tail <arquivo>        # últimas 10 linhas

## Busca e Filtros
grep "texto" arquivo  # busca uma palavra dentro do arquivo
find . -name "*.txt"  # busca arquivos pela extensão/nome no diretório atual

## Edição no Terminal
nano <arquivo>        # abre o editor de texto nano
vim <arquivo>         # abre o editor de texto vim (avançado)

## Permissões
chmod +x <arquivo>    # torna executável
chmod 755 <arquivo>   # permissão padrão

## Processos
ps aux                # lista processos
kill <pid>            # encerra processo
top                   # monitor de processos

## Rede
ping <host>           # testa conexão
curl <url>            # requisição HTTP
