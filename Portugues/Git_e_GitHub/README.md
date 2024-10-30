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