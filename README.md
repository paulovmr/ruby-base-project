ruby-base-project
=================

Instalando o RVM
================

# Baixar e instalar o RVM
curl -sSL https://get.rvm.io | bash -s stable

Instalando o Ruby
=================

# Abrir nova janela do terminal e instalar o Ruby 2.1.1
rvm install 2.1.1

# Conferir se versão foi instalada
rvm list

# Escolher qual versão usar
rvm use ruby-2.1.1

# Conferir qual versão do ruby está atualmente setada
ruby -v

# Abrir console do ruby
irb

# Mostrar GEMs instaladas na máquina
gem list

Aplicação de exemplo com Sinatra
================================

# Instalar a GEM Sinatra
gem install sinatra

# Criando arquivo
vim app.rb

require 'sinatra'

get '/' do
  'Hello World'
end

# Subir aplicação
ruby app.js

# Modificando arquivo
vim app.rb

require 'sinatra'

get '/' do
  "Hello, #{params[:nome]}"
end

