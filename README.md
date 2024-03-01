# xdebug-example
Este é um projeto simples criado como referência inicial para configuração do Xdebug em projetos PHP usando Docker e Docker Compose. Ele fornece uma estrutura mínima que você pode usar como ponto de partida para configurar e testar o Xdebug em seu ambiente local.

## Pré-requisitos
Antes de começar, certifique-se de ter os seguintes requisitos instalados em seu sistema:

 - Docker
 - Docker Compose

## Instalação e Uso

Clone este repositório para o seu ambiente local:

```bash
git clone https://github.com/danielsdev/xdebug-example.git
```

Navegue até o diretório do projeto:

```bash
cd projeto-xdebug-referencia
```

Inicie os containers docker usando o docker compose:

```bash
docker-compose up -d
```

Se precisar acessar o container da aplicação, use o comando:

```bash
docker-compose exec -it php bash
```

Abra seu editor de código e configure o Xdebug para se conectar ao host e à porta configurada no arquivo docker-compose.yml.

Use o script PHP simples (index.php) para testar a funcionalidade do Xdebug. Você pode adicionar breakpoints neste script e usar um depurador para inspecionar o código enquanto ele é executado.

Depois de concluir, pare o container docker:

```bash
docker-compose down
```

## Configuração do Xdebug

Se precisar alterar a configuração do Xdebug, basta editar o arquivo 90-xdebug.init

## Contribuindo
Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas ou enviar solicitações de pull com melhorias, correções de bugs ou novos recursos.

## Licença
Este projeto está licenciado sob a MIT License.
