# Backup no GitHub

## Atualizar a lista de pacotes do sistema:

apt update

Esse comando atualiza a lista de pacotes disponíveis no sistema. Isso é importante para garantir que você esteja instalando as versões mais recentes dos pacotes.

# Instalar os pacotes git e gh:

apt install -y git gh

git: Ferramenta de controle de versão distribuído.

gh: GitHub CLI, uma ferramenta de linha de comando para interagir com o GitHub.

A opção -y faz com que o apt aceite automaticamente todas as solicitações de confirmação durante a instalação.

## Criar um novo projeto MkDocs:

mkdocs new gsi-doc

Esse comando cria uma nova estrutura de projeto MkDocs chamada gsi-doc. O MkDocs é uma ferramenta de geração de documentação estática.

## Entrar no diretório do projeto:

cd gsi-doc

Esse comando muda o diretório atual para o diretório gsi-doc, onde você irá trabalhar com o projeto.

## Inicializar um repositório Git:

git init .

Esse comando inicializa um novo repositório Git no diretório atual. O ponto . indica que o repositório deve ser inicializado no diretório atual.

## Verificar o status do repositório:

git status

Mostra o status dos arquivos no repositório, incluindo arquivos que foram modificados e arquivos que estão prontos para o commit.

## Adicionar todos os arquivos ao repositório:

git add .

Esse comando adiciona todos os arquivos no diretório atual ao índice do Git, preparando-os para o commit.

## Verificar o status do repositório novamente:

git status

Verifica novamente o status dos arquivos para confirmar que todos foram adicionados.

## Fazer o commit dos arquivos:

git commit -m 'Primeira importação'

Cria um commit com a mensagem "Primeira importação". Um commit é uma captura das mudanças feitas no repositório.

## Autenticar-se no GitHub CLI:

gh auth login

Esse comando inicia o processo de autenticação para a GitHub CLI, permitindo que você se conecte à sua conta do GitHub.

## Criar um novo repositório no GitHub:

gh repo create gsi-doc --private

Esse comando cria um novo repositório no GitHub com o nome gsi-doc e define o repositório como privado. O repositório será associado ao projeto local.

## Adicionar a URL do repositório remoto:

git remote add origin https://github.com/USUARIO/gsi-doc

Esse comando adiciona um repositório remoto chamado origin, que aponta para a URL do repositório no GitHub. Substitua USUARIO pelo seu nome de usuário do GitHub.

## Enviar os commits para o repositório remoto:

git push -u origin main

Esse comando envia os commits da branch main do repositório local para o repositório remoto no GitHub. A opção -u define origin/main como a branch padrão para futuros pushes e pulls.

## Sair da autenticação do GitHub CLI:

gh auth logout

Esse comando encerra a sessão de autenticação com a GitHub CLI. É uma boa prática sair da sessão quando você terminar o trabalho para manter a segurança.

Esses passos configuram um novo projeto de documentação, inicializam um repositório Git, e enviam o projeto para um repositório privado no GitHub. 


