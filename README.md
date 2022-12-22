## 🪡 Geradores de CSS :rocket:	
> Geradores de CSS para o seu projeto.
- [UI Verse](https://uiverse.io/) - Gerador de buttons, checkboxes, toggle switches, cards, loaders, inputs. <br>
- [Neumorphism](https://neumorphism.io/) - Tendência aplicação border-radius <br>
- [Fancy Border-Radius](https://9elements.github.io/fancy-border-radius/) - Gerador de formas com border-radius no CSS <br>
- [WAIT! Animate](https://waitanimate.wstone.io) - Gerador de animações de CSS <br>
- [Best CSS Button Generator](https://www.bestcssbuttongenerator.com) - Gerador de botões do CSS <br>
- [HTML CSS JS Generator](https://html-css-js.com/css/generator/) - Gerador de HTML/CSS/JS <br>
- [BennettFeely](https://bennettfeely.com/clippy/) - Criador de clip-path <br>
- [Animista](https://animista.net) - Criador de animações <br>
- [Layoutit](https://grid.layoutit.com/) - Gerador de Grid para CSS <br>
- [CSS Gradient](cssgradient.io) - Gerador de gradientes <br>
- [Keyframes](keyframes.app) - Site ajuda você a criar animações keyframes básica e complexas <br>
- [Glassmorphism](css.glass) - Site é usado para criar estética de vidro e gerar código CSS <br>
- [SVG Wave Generator](getwaves.io) - Um gerador de ondas SVG gratuito <br>
- [Bob SVG Generator](blobmaker.app) - Site para criar formas SVG aleatórias, únicas e orgânicas <br>
- [Cubic Bezier](https://cubic-bezier.com/) - Ferramenta para Cubic-bezier() <br>
- [Shadow Generator](https://shadows.brumm.af/) - Gerador de sombras <br>
- [Glassmorphism CSS Generator](https://ui.glass/generator/) - Gerador de glassmorphism <br>
- [Grabient](grabient.com) - Gerador de gradientes <br>
- [Box Shadow](cssmatic.com/box-shadow) - Gerador de box-shadow <br> 
- [Box Shadows Dev](box-shadow.dev) - Gerador de box-shadow <br> 
- [Drop Shadow](webcode.tools/generatores/css/dropshadow) - Gerador de drop-shadow <br> 
- [CSS Bud](cssbud.com/css-generator/css-box-shadow-generator/) - Gerador de box-shadow  <br> 
- [Shadow Palette](joshwcomeau.com/shadowpalette) - Gerador de sombras. <br> 



# Tutorial-github-bash
Comandos e como Funciona o Github-bash

![img](https://github.githubassets.com/images/modules/site/social-cards/github-social.png)


### Primeiros passos
- Criar uma conta pessoal no GitHub
- Instalar Git Client
  - https://git-scm.com/downloads
- Criar um novo repositório no Github
- Criar assinatura
  - 
  ```
  git config --global user.name "Seu usuario"
  git config --global user.email "email@example.com
  ```
- Clonar repositório
  - 
  ``` 
  git clone <url_repositorio>
  ```
  
  ## Comandos Git
  
<br/>

### Git Help

```
git help
git help <comando> #Comando o qual deseja maiores informações
```

O comando help irá lhe mostrar qual a função de determinado comando e quais opções podem ser utilizadas junto com aquele comando.   

#### Git Clone  
```
git clone <endereco-repositorio-remoto>
```
O Git clone é um comando para baixar o código-fonte existente de um repositório remoto (como o Github, por exemplo). Utilizando GitHub é possível fazer o *git clone* por https ou ssh.

#### Git Init
```
git init
```

Cria um novo repositório local Git. Com esse comando será criado um novo subdiretório chamado .git que contem todos os arquivos necessários de seu repositório — um esqueleto de repositório Git.  

### Git Remote

```
git remote add origin <endereco_repositorio>
```

Vincula o repositório local a um repositório remoto.


```
git remote
git remote -v
```

Exibe os repositórios remotos.  


#### Git Status  
```
git status
```
Fornece todas as informações necessárias sobre o branch atual, como por exemplo ficheiros que sofreram alterações que podem ser incluídos no próximo *commit*.  

#### Git Add
```
git add <ficheiro>
git add .
```  
Adiciona um ficheiro ou todos o ficheiros que sofreram modificações e/ou foram incluídos no  próximo *commit*.
Este comando não altera o repositório, as alterações não são salvas até fazermos um *commit*. 

#### Git Restore
```
git restore --staged <ficheiro>
```  
Remove do próximo *commit* ficheiro que foi incluído no  próximo *commit*.

```
git restore <ficheiro>
```  
Restaura o ficheiro para o última estado dele na Branch. Cuidado, isso irá remover todas suas alterações que não foram *committed*.

#### Git Reset

```
git reset HEAD <ficheiro>
```

Remove do próximo *commit* ficheiro que foi incluído no  próximo *commit*. (igual ao comando *git restore --staged*)


```
git reset --hard
```

Retorna o repositório para o último commit na branch a qual está posicionado. Cuidado, todas as suas alterações que não foram *committed* serão perdidadas.

#### Git Commit

```
git commit -m "Mensagem explicativa da alteração realizada"
```
Este comando é como definir um ponto de verificação no processo de desenvolvimento, para o qual você pode voltar mais tarde se necessário. Quando é feito o *git commit* as alterações são confirmadas apenas no repositório local.  

#### Git Push
```
git push <remote> <nome-do-branch>
git push origin main
```
Este comando é utilizado para enviar o commit da sua branch no repositório local para uma branch em um repositório remoto.

#### Git Pull
```
git pull <remote>
git pull origin
git pull
```

Obtém atualizações do repositório remoto, quando usamos o git pull, ele recebe as atualizações do repositório remoto e aplica imediatamente as alterações mais recentes no seu repositório local.  

#### Git Branch

Com branches, vários desenvolvedores podem trabalhar em paralelo no mesmo projeto simultaneamente.

Pode-se usar o comando git branch para criar, listar e excluir branches.

```
git branch <nome-do-branch>
```

Cria nova branch.

```
git branch
git branch --list
```

Lista branches.


```
git branch -d <nome-do-branch>
```

Deleta branches.


```
git push -u <remote> <nome-da-branch>
```   

Replica branch para o repositório remoto.


```
git branch --merged
```   

Lista branches que já foram fundidos (merged) com o master. 

```
git branch --no-merged
```

Listar branches que não foram fundidos (merged) com o master.

#### Git Checkout

Este é um dos comandos Git mais usados. Para trabalhar em uma branch, primeiro você precisa mudar para ela.

Usamos o git checkout principalmente para alternar de um branch para outro. Também podemos usá-lo para verificar arquivos e commits.

```
git checkout <nome-do-branch>
```
Altera árvore de trabalho para outra branch.


```
git checkout -b <nome-da-branch>
```

Cria um novo branch e fazer checkout ao mesmo tempo.

#### Git Log  

```
git log
```   

Exibe histórico do repositório

```
git log -p -2
```

Exibe histórico com diff das duas últimas alterações.  


```
git log --stat
```   

Exibe resumo do histórico (hash completa, autor, data, comentário e qtde de alterações (+/-))   


```
git log --pretty=oneline
```

Exibe informações resumidas em uma linha (hash completa e comentário)  

```
git log --diff-filter=M -- <ficheiro>
```

Exibe histórico modificação de um ficheiro  


#### Git Tags

Tags são utilizadas normalmente para marcar um ponto que determina a versão da aplicação, desta forma, é possível seguir na mesma branch principal e conseguir voltar para pontos de versão apenas utilizando as tags.

```
git tag v1.1 -m "descricao"
```  
Cria uma tag localmente, a tag é criada na branch onde estiver no momento em que executar o comando. 
  


```
git push origin <tag_name>
```  

Criar a tag que foi criada localmente no repositório remoto.


```
git push origin --tags
``` 

Cria todas as tags locais no repositório remoto.

#### Git Merge

O git merge permite fazer um merge entre duas branch.

```
git merge <branch_a_realizar_merge>
```

Para realizar o merge, é necessário estar no branch que deverá receber as alterações. O merge pode acontecer de forma automática ou exigir uma ação manual. O merge automático será feito em arquivos textos que não sofreram alterações nas mesmas linhas, já o merge manual será feito em arquivos textos que sofreram alterações nas mesmas linhas, onde será necessário intervenção e realização de um novo commit após esta intevenção.

---
