# Diario de bordo

## 1 - Dia não

**Estruturas de pastas**

- app - Possui os controlers, models, views, helpers, mailrs, jobs, e assets. 
- bin - Contem os scripts, os deploy, updates, e as coisas para rodar a aplicaçao "os comandos"
- config - Aqui configura as rotas, o database, e mais
- config.ru - Iniciar o app usando Rack
- db - guardar os templates do database
- Dockerfile - é o dockerfile
- Gemfile e Gemfile.lock - Usando tipo o packjson do npm, é pra pegar as depedencias e essas coisas ai
- lib - Extensao dos modulos
- log - Logs do app
- public - Files estaticos, exposostor e publicos
- rakefile - Este arquivo localiza e carrega tarefas que podem ser executadas a partir da linha de comando. As definições de tarefas são definidas em todos os componentes do Rails. Em vez de alterar o Rakefile, você deve adicionar suas próprias tarefas adicionando arquivos ao diretório lib/tarefas do seu aplicativo.
- script - Contem scripts
- storage - Guarda o SQLite databases e arquiqovos no disco
- test - Para tests unitarios
- vendor - Um lugar para todo o código de terceiros. Em um aplicativo típico Rails, isso inclui gemas de fornecedores.
- kamal - Contém segredos do Kamal e ganchos de implantação.

### Criando um database

Para criar o database 

```bash
bin/rails db:create
```

Iniciar o server 

```bash
bin/rails server
```

#### Criando um model

```bash
bin/rails generate model Product name:string
```
Rorando a migratino
```bash
bin/rails db:migrate
```
#### Console log
Ativa um console para o rails, que voce pode controlar o banco de dados diretamente por ele
manual de como usar o [console](https://guides.rubyonrails.org/getting_started.html#active-record-model-basics)

```bash
bin/rails console
```