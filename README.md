
# Projeto criado com o objetivo de utilizar o Ansible para provisionar toda infra estrutura de um ambiente de monitoramento utilizando o Prometheus + Grafana + Alertmanager utilizando o Docker.

## HOSTS
Para executar essa playbook será necessário como primeiro passo ajustar o arquivo 'hosts' dentro do diretório "*inventory*" para informar qual será o servidor que a role executará as tarefas.

A role **ansible-docker** realizar a instalação do docker e docker-compose e em seguida executa o arquivo docker-compose.yml e provisiona os seguintes containeres:

- prometheus
- alertmanager
- grafana
- node-exporter
- cAdvisor
- Apache


Na pasta **configs** estão todos os arquivos de configuração das aplicações listadas acima, edite os arquivos de acordo com o seu ambiente.

## Validado em ambientes Debian 10.
## Embreve para ambietes CentOS 8.

Criado por [Rauny Moreira](https://www.linkedin.com/in/rauny-moreira/).
