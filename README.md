Olá pessoal!

Para usar as ferramentas que trabalharemos na aula seguinte para compilar os protofiles será necessário instalar alguns pacotes.

Hoje podemos unificar a instalação dos pacotes nos sistemas operacional, porque no Windows existe o WSL (Windows Subsystem for Linux). Se você ainda não configurou este ambiente no seu Windows, vá no módulo de Docker e veja o primeiro capítulo.

Execute estes comandos no seu terminal Linux/MAC:

sudo apt install protobuf-compiler 
brew install protobuf #Mac, requer Homebrew instalado
go get google.golang.org/protobuf/cmd/protoc-gen-go google.golang.org/grpc/cmd/protoc-gen-go-grpc
Para finalizar, temos que adicionar a pasta "/go/bin" no PATH do Linux para que tudo que seja instalado nesta pasta esteja disponível como comandos no terminal. Adicione no final do seu ~/.bash

PATH="/go/bin:$PATH"
Execute o comando abaixo para atualizar seu terminal:

source ~/.bashrc
Pronto, todos os executáveis usados na aula anterior já estão disponíveis no seu terminal.

É isso aí pessoal, até a próxima.