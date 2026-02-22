# Projeto-Conceitual

## 🛒 Projeto Conceitual – E-commerce (Desafio DIO)
📖 Descrição

Neste desafio foi modelado um contexto reduzido de um sistema de E-commerce, aplicando conceitos de modelagem conceitual de banco de dados.

A ferramenta escolhida para modelagem foi o MySQL Workbench, utilizando diagrama EER (Enhanced Entity Relationship).

Mesmo sendo um modelo conceitual, foram especificadas as PKs (Primary Keys) e FKs (Foreign Keys) conforme orientação do desafio, garantindo clareza na definição dos relacionamentos.

## 🎯 Objetivo do Desafio

Construir o esquema conceitual de um sistema de E-commerce contendo:

Cliente PF e PJ (especialização exclusiva)

Pedido

Pagamento (múltiplas formas)

Entrega (com status e código de rastreio)

## 🧩 Regras de Negócio Aplicadas
🔹 Cliente

Um cliente pode ser Pessoa Física (PF) ou Pessoa Jurídica (PJ).

A especialização é:

Total

Exclusiva

🔹 Pedido

Um cliente pode realizar vários pedidos.

Cada pedido pertence a um único cliente.

🔹 Pagamento

Um cliente pode cadastrar mais de uma forma de pagamento.

Cada pagamento pertence a um único cliente.

🔹 Entrega

Cada pedido possui uma entrega.

A entrega possui:

Status

Código de rastreio

## 🗂 Estrutura das Entidades
Cliente (Superclasse)

id_cliente (PK)

email

telefone

Cliente_PF

id_cliente (PK e FK)

nome

cpf

data_nascimento

Cliente_PJ

id_cliente (PK e FK)

razao_social

nome_fantasia

cnpj

Pedido

id_pedido (PK)

data_pedido

valor_total

status_pedido

id_cliente (FK)

Pagamento

id_pagamento (PK)

tipo_pagamento

valor

data_pagamento

id_cliente (FK)

Entrega

id_entrega (PK)

status_entrega

codigo_rastreio

id_pedido (FK)


## 🛠 Tecnologias Utilizadas

MySQL Workbench

Modelo EER

SQL (para definição estrutural)


## 📌 Entregáveis

Diagrama conceitual (modelo EER)

Script SQL de criação das tabelas

Documentação das regras de negócio

