# CryptoSQL

Este script foi adaptado para coletar, enviar e armazenar dados de preços de criptomoedas em diferentes moedas usando o Yahoo Finance API. O script é executado em um loop infinito, coletando dados a cada 5 segundos e enviando-os para um tópico Kafka e salvando-os em um banco de dados MySQL usando SQL Alchemy.

## Configurações

Antes de executar o script, você deve configurar as seguintes variáveis de ambiente:

### Cryptomoedas

Defina as criptomoedas que deseja coletar dados. Atualmente, o script está configurado para coletar dados para BTC, ETH e LTC.

```python
crypto_list = ["BTC-USD", "ETH-USD", "LTC-USD"]
```

## Moedas

Defina as moedas nas quais deseja obter os preços. Atualmente, o script está configurado para obter preços em USD, EUR, ARS e BRL.

```
currency_list = ["USD", "EUR", "ARS", "BRL"]
```

## Apache Kafka

Defina as configurações do Apache Kafka para enviar dados para um tópico.

## MySQL

Defina as configurações do MySQL para armazenar dados.

```
db_username = 'seu_usuario'
db_password = 'sua_senha'
db_host = 'localhost'
db_name = 'crypto_data'
```

## Execução

Para executar o script, basta rodar o arquivo python. O script será executado em um loop infinito, coletando, enviando e armazenando dados a cada 5 segundos.

```
CryptoSQL.ipynb
```
