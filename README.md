# Modelagem de Banco de Dados Relacional com MySQL Workbench

Este repositório reúne meus estudos sobre **modelagem de banco de dados relacional**, utilizando o **MySQL Workbench** para criação de Diagramas Entidade-Relacionamento (DER) e implementação em **MySQL**.

O objetivo é compreender como estruturar bancos de dados consistentes, aplicando conceitos como entidades, relacionamentos, chaves primárias, chaves estrangeiras, cardinalidade e integridade referencial.

---

##  Diagrama do Banco de Dados

Abaixo está o modelo desenvolvido durante os estudos:

<img width="1647" height="953" alt="Captura de tela 2026-07-16 164321" src="https://github.com/user-attachments/assets/a20a5c5a-547d-4109-8876-2c3433077168" />


---

# Conceitos Aplicados

## Entidades

As entidades representam objetos do mundo real que precisam ser armazenados no banco de dados.

**Exemplos do projeto:**

- `produto`
- `categoria`
- `programador`
- `projeto`
- `programador_projeto`

Cada entidade é transformada em uma tabela dentro do banco de dados.

---

## Chave Primária (Primary Key)

A chave primária identifica exclusivamente cada registro de uma tabela.

Exemplos:

- `produto.id`
- `categoria.idcategoria`
- `programador.idprogramador`
- `projeto.idprojeto`

A chave primária garante que não existam registros duplicados.

---

## Chave Estrangeira (Foreign Key)

A chave estrangeira estabelece o relacionamento entre tabelas.

Ela referencia a chave primária de outra tabela, garantindo a integridade dos dados.

Dessa forma, não é possível associar um programador inexistente a um projeto.

---

# Relacionamentos

### Relacionamento 1:N (Um para Muitos)

Representa quando um registro pode estar relacionado a vários registros da outra tabela.



### Relacionamento N:M (Muitos para Muitos)

Esse relacionamento ocorre quando várias ocorrências de uma entidade podem se relacionar com várias ocorrências de outra.

No banco de dados relacional, esse relacionamento é implementado por meio de uma **tabela associativa**.


---

#  Cardinalidade

A cardinalidade define a quantidade de registros que podem participar de um relacionamento.

No modelo foram utilizados:

- **1:N (Um para Muitos)**
- **N:M (Muitos para Muitos)**

Esses conceitos são fundamentais para manter o banco organizado.

---

# Integridade Referencial

Durante a implementação do modelo foi possível compreender a importância da integridade referencial.

Ao criar uma chave estrangeira, o MySQL exige que:

- o tipo de dado seja exatamente igual;
- o tamanho seja compatível;
- atributos como **UNSIGNED** também sejam iguais.

Durante os estudos encontrei o seguinte erro:

> Referenced table has no candidate columns with a compatible type

O problema foi resolvido ajustando a coluna da chave estrangeira para possuir exatamente o mesmo tipo da chave primária da tabela referenciada.

---

#Objetivos do Projeto

- Praticar modelagem de banco de dados.
- Compreender relacionamentos entre tabelas.
- Aplicar chaves primárias e estrangeiras.
- Trabalhar com cardinalidade.
- Garantir integridade referencial.
- Utilizar o MySQL Workbench para modelagem visual.

---

# Tecnologias Utilizadas

- MySQL Workbench


---

# Aprendizados

Este projeto foi desenvolvido como parte dos meus estudos em banco de dados durante o curso Técnico em Desenvolvimento de Sistemas e o Bacharelado em Engenharia de Software.

A proposta é consolidar os fundamentos da modelagem relacional antes do desenvolvimento de aplicações que utilizam bancos de dados.

---

##Autor

**Bruno Henrique Rodrigues**

- LinkedIn: https://linkedin.com/in/thedevbrun0
- GitHub: https://github.com/thedevbrun0
