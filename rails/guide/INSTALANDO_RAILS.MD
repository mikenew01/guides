# INSTALANDO RAILS

### Ruby On Rails no Windows
1. **Download do Rails Installer:**
    - Faça o download do instalador clicando [aqui](http://www.railsinstaller.org/pt-BR)
2. **Instalação do Rails Installer:**
    - Instalação padrão.

### Ruby On Rails no Ubuntu 17.04:
1. **Instalando Dependências:**
    1. Atualizando pacotes:
    ```shell
    sudo apt update -y && sudo apt upgrade -y
    ```
    2. Instalando Dependências:
    ```shell
    sudo apt install -y git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev 
    libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev 
    python-software-properties libffi-dev nodejs
    ```
2. **Instalando Gerenciador de Versões:**
    1. Instalando Rbenv: 
    ```shell
    cd
    git clone https://github.com/rbenv/rbenv.git ~/.rbenv
    echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
    echo 'eval "$(rbenv init -)"' >> ~/.bashrc
    exec $SHELL

    git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
    echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
    exec $SHELL
    ```
    2. Instalando Ruby 2.4.1:
    
    ```shell
    rbenv install 2.4.1 #Sua versão
    rbenv global 2.4.1 #Sua versão
    ruby -v
    ```
    
    > OBS: Utilize `rbenv local 2.4.1` para definir versão local.
    
3. **Instalando Bundler:**
    ```shell
    gem install bundler
    ```
    
4. **Instalando NodeJS:**
    1. NodeJS 6.x (Recomendado):
    ```shell
    curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
    sudo apt install -y nodejs
    ```
5. **Instalando Rails 5.1.1:**
    ```shell
    gem install rails -v 5.1.1 #Sua versão
    ```
6. **Verificando versão do Rails:**
    ```shell
    ruby  -v
    rails -v
    ```
