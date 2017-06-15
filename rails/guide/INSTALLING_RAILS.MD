# INSTALLING RAILS

![Rails](images/ror.png)

### RUBY ON RAILS IN UBUNTU 17.04
1. **Installing Ruby 2.4.1:**
    ```shell
    sudo apt update -y && sudo apt upgrade -y
    sudo apt install -y git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev 
    libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev 
    python-software-properties libffi-dev nodejs
    ```
2. **Installing Rbenv:**
    ```shell
    cd
    git clone https://github.com/rbenv/rbenv.git ~/.rbenv
    echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
    echo 'eval "$(rbenv init -)"' >> ~/.bashrc
    exec $SHELL

    git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
    echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
    exec $SHELL

    rbenv install 2.4.1 #Your version
    rbenv global 2.4.1 #Your version
    ruby -v
    ```
3. **Installing Bundler:**
    ```shell
    gem install bundler
    ```
    
4. **Installing Dependencies:**
    - NodeJS 4.x:
    ```shell
    curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
    sudo apt install -y nodejs
    ```
    **or**
    
    - NodeJS 6.x (Recommended):
    ```shell
    curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
    sudo apt install -y nodejs
    ```
5. **Installing Rails 5.1.1:**
    ```shell
    gem install rails -v 5.1.1 #Your version
    ```
6. **Rails Version:**
    ```shell
    rails -v
    ```
