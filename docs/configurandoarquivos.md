# Configurando os arquivos

Copiar e alterar o arquivo (000-default.conf) com nome (www.conf e docs.conf) no diretório /etc/apache2/sites-available.

  - `cd /etc/apache2/sites-available`

  - `cp 000-default.conf  www.conf`

  - `cp 000-default.conf  docs.conf`

OBS: 

-  Alterar o Documentroot para o seu diretório do seu site

-   Ex: Documentroot:  /var/www/diretório_do_site

-   Altere o NameServer para o url que você deseja para o seu site

EX: NameServer www.exemplo.lab

Ficara assim no `www.antenor.lab.conf`

Nesse exemplo o diretório do meu site se chama 'Antenor'.

OBS: No caso da criação de um site usando o (mkdocs) o documentroot apontara dessa forma:

-   Ex: Documentroot:  /var/www/docs/site

Fazer um link de (www.conf e docs.conf) para /etc/apache2/sites-enabled.

-   `cd /etc/apache/sites-enabled`

-   `ln -s /etc/apache2/sites-available/www.conf`

-   `ln -s /etc/apache2/sites-available/docs.conf`

ou

-   a2ensite nome_do_arquivo

```
<VirtualHost *:80>
    ServerName docs.antenor.lab
    DocumentRoot /var/www/html/antenor/

    <Directory /var/www/html/antenor/>
        Options Indexes FollowSymLinks MultiViews
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>

```

```
VirtualHost *:80>

        ServerName www.antenor.lab

        ServerAdmin webmaster@localhost
        DocumentRoot /var/www/html/apple/wordpress/

        ErrorLog ${APACHE_LOG_DIR}/error.log
        CustomLog ${APACHE_LOG_DIR}/access.log combined

</VirtualHost>



```
