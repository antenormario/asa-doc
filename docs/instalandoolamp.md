# Instalando o LAMP

Nessa primeira primeira etapa é feita as instalações das dependencias para o nosso site, conhecida como LAMP. Além das dependências precisaremos do curl para baixar o wp-cli e o mkdocs para documentar o nosso site.

## O Que É LAMP?

LAMP é um acrônimo para um conjunto de software que é frequentemente usado para criar servidores web. O conjunto é composto por:

Linux: O sistema operacional.
Apache: O servidor web.
MySQL ou MariaDB: O sistema de gerenciamento de banco de dados.
PHP: A linguagem de programação usada para desenvolver aplicações web.

# O Que Cada Pacote Faz?

Vamos detalhar o que cada um dos pacotes listados faz:

apache2: Este é o servidor web Apache. Ele é responsável por receber e processar as solicitações HTTP dos navegadores e servir as páginas web para os usuários.

php: PHP é uma linguagem de programação do lado do servidor. É amplamente usada para criar páginas web dinâmicas e interativas.

mariadb-server: Este é o servidor de banco de dados MariaDB, que armazena dados do site. MariaDB é uma alternativa ao MySQL e é bastante compatível com ele.

libapache2-mod-php: Este módulo permite que o Apache interprete e execute scripts PHP. Sem este módulo, o Apache não seria capaz de processar páginas PHP.

php-mysql: Este pacote fornece a extensão PHP para se conectar e interagir com bancos de dados MySQL/MariaDB. É necessário para que scripts PHP possam usar o banco de dados.

curl: cURL é uma ferramenta de linha de comando e uma biblioteca para transferir dados com URLs. Ele é usado aqui para baixar o wp-cli, que é uma ferramenta de linha de comando para gerenciar instalações do WordPress.

mkdocs-*: MkDocs é uma ferramenta de documentação que gera sites a partir de arquivos Markdown. O mkdocs-* no comando indica que você está instalando o MkDocs e talvez alguns plugins ou extensões associados.

## Comando para Instalação

O comando que você forneceu é:

`apt install -y apache2 php mariadb-server libapache2-mod-php php-mysql curl mkdocs-*`

### Aqui está o que cada parte faz:

apt install: Este é o comando para instalar pacotes no sistema baseado em Debian/Ubuntu.

-y: Esta opção automaticamente responde "sim" a todas as perguntas durante a instalação, o que permite a instalação não-interativa.

apache2 php mariadb-server libapache2-mod-php php-mysql curl mkdocs-*: Estes são os pacotes a serem instalados. O mkdocs-* é uma expressão curinga que instala o MkDocs e qualquer pacote que comece com mkdocs-.

## Em Resumo

Este comando instala todos os componentes necessários para configurar um servidor web básico com o LAMP stack e também inclui ferramentas adicionais para gerenciar WordPress e documentar o site. Após executar este comando, você terá:

- Um servidor web Apache em funcionamento.
- Suporte para PHP e integração com o banco de dados MariaDB.
- Ferramentas adicionais como curl para downloads e mkdocs para documentação.

