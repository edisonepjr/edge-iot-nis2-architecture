# Arquitetura Edge-IoT Resiliente

## Visão Geral

A arquitetura proposta utiliza um cluster distribuído de dispositivos ESP32 com um gateway central baseado em Raspberry Pi Zero W.

## Componentes

### Nós Sensores (ESP32)
- Coleta de dados ambientais
- Validação local
- Criptografia AES-256-GCM
- Armazenamento temporário (buffer)

### Gateway (Raspberry Pi Zero W)
- Agregação de dados
- Interface com serviços externos
- Gerenciamento do cluster

## Comunicação

- Protocolo leve (ex: MQTT/HTTP)
- Modelo store-and-forward
- Tolerância a falhas de rede

## Segurança

- Secure Boot ativado
- Flash encryption
- Desativação de interfaces de debug
- Gestão de chaves local

## Resiliência

- Operação offline com buffer local
- Sincronização automática após reconexão
- Recuperação de 100% dos dados em testes controlados

## Escalabilidade

- Arquitetura modular
- Possibilidade de expansão do cluster
- Baixo custo por nó
