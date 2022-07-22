<h1 style='text-align: center;'>Configurar e subir o ambiente localmente</h1>

## Introdução

Este guia tem como objetivo auxiliar novos desenvolvedores a subirem pela primeira vez a aplicação completa localmente, bem como auxiliar os demais desenvolvedores a subirem e derrubarem a aplicação de forma mais simples.

> Este guia se destina a desenvolvedores com ambiente Linux

## Baixando os fontes do projeto

Em uma pasta de sua escolha (preferencialmente alguma que não exija privilégios de administrador), crie uma pasta para acomodar os fontes do projeto e entre nela:

```bash
mkdir siged && cd siged
```

Execute o seguinte comando para baixar todos os arquivos do projeto provenientes do _GitHub_:

```bash
git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Frontend && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Clients && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Users && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Demands && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Sectors && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Cargos
```

## Dependências

Como o ambiente será executado dentro de um container [`docker`](https://www.docker.com/), é necessário que se siga os passos de instalação disponibilizados neste [guia](https://docs.docker.com/engine/install/ubuntu/) caso você ainda não tenha o _Docker_ em sua máquina. Em máquinas com sistema _Linux_, é necessário seguir o guia de [_pós instalação_](https://docs.docker.com/engine/install/linux-postinstall/).

## Subindo a aplicação

Dentro da pasta `siged` onde estão as pastas da aplicação, rode o seguinte _script_ para subir a aplicação:

```sh
docker network create siged_backend
for dir in 2021-2-SiGeD-Cargos 2021-2-SiGeD-Demands 2021-2-SiGeD-Sectors 2021-2-SiGeD-Clients 2021-2-SiGeD-Frontend 2021-2-SiGeD-Users
do
  docker-compose --f ./${dir}/docker-compose.yml up --detach
done
```

É recomendado que se crie um arquivo para salvar este _script_ e utilizá-lo posteriormente de forma mais eficaz. Ainda dentro da pasta, crie um arquivo chamado `initialize_containers.sh` e cole o _script_ dentro dele.

Utilizando o `bash`, para executar este _script_, utilize o comando:

```bash
bash initialize_containers.sh
```
## Derrubando a aplicação

Dentro da pasta onde estão as pastas da aplicação, para derrubar a aplicação rode o seguinte _script_:

```sh
for dir in 2021-2-SiGeD-Cargos 2021-2-SiGeD-Demands 2021-2-SiGeD-Sectors 2021-2-SiGeD-Clients 2021-2-SiGeD-Frontend 2021-2-SiGeD-Users
do
  docker-compose --f ./${dir}/docker-compose.yml down
done
docker network rm siged_backend
```

Assim como o _script_ de inicialização do container, é recomendado criar um arquivo para acomodar o _script_ que derruba a aplicação. Crie um arquivo chamado `stop_containers.sh` e cole o _script_ dentro dele.

Utilizando o `bash`, para executar este _script_, rode o seguinte comando:

```bash
bash stop_containers.sh
```