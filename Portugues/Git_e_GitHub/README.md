# GIT E GITHUB

---

## Inicializando um repositório

Para iniciar um repositório basta usar o comando `git init` dentro do diretório que deseja.

![Git Init](img/git_init.png)

---

## Status do projeto

Utilize o `git status` para observar o estado dos arquivos que estão dentro do repositório.

![Git Status](img/git_status.png)

---

## Git ignore

Caso queira deixar algum tipo de arquivo ou repositório escondido do git utilize um arquivo `.gitignore`. Caso tenha outros arquivos que queira ignorar basta colocar o nome dos arquivos dentro do arquivo `.gitignore`.

![.GitIgnore](img/gitignore.png)

---

## Identificação de usuario

Quando vamos commitar uma arquivo, precisamos nos identificar para saber qual pessoa fez tal commit. Por isso usamos os comandos `git config user.name "Nome"` e `git config user.email "Email"`.


> - ### Configurando localmente 
>>`git config user.name "Nome Sobrenome"`
>>
>>`git config user.email "email@gmail.com"`
> 
>É recomendavel usar esse tipo de identificação caso o computador que você use seja utilizado por mais pessoas alem de você.

> - ### Configurando globalmente
>>`git config --global user.name "Nome Sobrenome"`
>>
>>`git config --global user.email "email@gmail.com"`
>
>É recomendavel usar esse tipo de identificação caso o computador que você use seja utilizado somente por você.

---

## Git add

O comando `git add` é usado para notificar o git que ele vai monitorar esse arquivo.

> - ### Adicionar arquivos separadamente
>> `git add (nome do arquivo)`
>
> - ### Adicionar todos os arquivos modificados
>> `git add .`

---

## Git commit

O `git commit` é usado para notificar que o arquivo foi salvo, nele você da uma breve explicação sobre oque foi modificado.

> `git commit -m "Commitando"`

---

## Git log

O `git log` é responsável por mostrar o histórico de commits feitos naquele repositório e os hashes (hash é o código de identificação do commit, que está destacado em amarelo)

![`git log`](img/gitlog.png)

> ### Filtragem de palavra

Caso eu queira fazer uma busca mais aprofundada nos logs do repositório, posso passar como parâmetro, após o `git log`, a palavra pela qual estou buscando.

`git log`
`/Atualização`

![`Busca aprofundada`](img/gitlog_busca_por_palavra.png)

> ### Filtragem de logs

Caso eu queira filtrar uma quantidade de logs.

`git log -2`

![Filtragem de logs](img/gitlog_filtragem.png)


### Filtrando commit's logs

Utilize o comand `git log --oneline`

![Oneline](img/gitlog_oneline.png)


### FIltragem por data


Podemos filtrar a partir da data com os comandos a seguir:
>`git log --after='dd-mm-yyyy'`
>`git log --before='dd-mm-yyyy'`
>`git log --since='2 days ago'`
>`git log --after='3 mounths ago'`
>`git log --before='1 year ago'`
>`git log --author='autor'`

![](img/gitlog_data.png)

### git help log

caso queira mais alguma ajuda use o comando `git help log`

---

## git checkout (hash)


Caso queiramos voltar um commit que fizemos, poderemos usar o `git checkout (código da hash)`, isso vai fazer o seu arquivo voltar no tempo. Ele ira recuperar os dados daquela data do commit e descartando a nova.


![](img/git_volta_no_tempo.png)

Para voltar para a main utilize `git checkout maste/main`


## Em produção...

