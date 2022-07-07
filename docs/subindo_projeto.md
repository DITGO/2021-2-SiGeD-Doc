<h1 style='text-align: center;'>Configurar e subir o ambiente localmente</h1>

## Baixando os fontes do projeto

Em uma pasta de sua escolha (preferencialmente alguma que não exija privilégios), crie uma pasta para acomodar os fontes do projeto:

```bash
mkdir siged && cd siged
```

Execute o seguinte comando para baixar todos os arquivos do projeto:

```bash
git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Frontend && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Clients && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Users && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Demands && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Sectors && git clone https://github.com/fga-eps-mds/2021-2-SiGeD-Cargos
```

## Subindo a aplicação

Para subir a aplicação, entre na pasta onde os arquivos foram baixados e crie um arquivo chamado `initialize_containers.sh`. Abra este arquivo e cole o seguinte script:

```sh
docker network create siged_backend

cd 2021-2-SiGeD-Cargos && docker-compose up --detach && cd ..
cd 2021-2-SiGeD-Demands && docker-compose up --detach && cd ..
cd 2021-2-SiGeD-Sectors && docker-compose up --detach && cd ..
cd 2021-2-SiGeD-Clients && docker-compose up --detach && cd ..
cd 2021-2-SiGeD-Frontend && docker-compose up --detach && cd ..
cd 2021-2-SiGeD-Users && docker-compose up --detach && cd ..
```

Para executar este script, utilize o comando:

```bash
bash initialize_containers.sh
```
## Derrubando a aplicação

Dentro da pasta que contém os arquivos da aplicação (`siged`) crie um arquivo chamado `stop_containers.sh` e então cole o seguinte script dentro deste arquivo:

```sh
cd 2021-2-SiGeD-Cargos && docker-compose down && cd ..
cd 2021-2-SiGeD-Demands && docker-compose down && cd ..
cd 2021-2-SiGeD-Sectors && docker-compose down && cd ..
cd 2021-2-SiGeD-Clients && docker-compose down && cd ..
cd 2021-2-SiGeD-Frontend && docker-compose down && cd ..
cd 2021-2-SiGeD-Users && docker-compose down && cd ..

docker network rm siged_backend
```

Para executar este script, rode o seguinte comando:

```bash
bash stop_containers.sh
```