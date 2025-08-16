# Modelo Conceitual de Banco de Dados para Oficina Mecânica

## Descrição do Projeto
Este projeto apresenta um **modelo conceitual de banco de dados para uma oficina mecânica**, permitindo o controle e gerenciamento de ordens de serviço. O sistema registra clientes, veículos, equipes de mecânicos, serviços realizados, peças utilizadas e o cálculo de valores de cada OS.

O modelo contempla:
- Controle de **clientes** (PF ou PJ) e seus veículos.
- Gestão de **equipes de mecânicos** e suas especialidades.
- Registro detalhado de **ordens de serviço**, incluindo serviços realizados e peças utilizadas.
- Cálculo automático do **valor total da OS** com base em serviços e peças.

---

## Diagrama Conceitual

![Esquema Conceitual para Banco De dados](Esquema%20Conceitual%20para%20Banco%20De%20dados.jpg)

> A imagem acima representa todas as entidades, atributos e relacionamentos do modelo conceitual da oficina mecânica.

---

## Entidades Principais
1. **Cliente**: ID, nome, endereço, telefone, tipo (PF/PJ)  
2. **Veículo**: ID, placa, modelo, marca, ano, ID do cliente  
3. **Mecânico**: ID, nome, endereço, especialidade  
4. **Equipe**: ID, nome da equipe, composta por mecânicos  
5. **Ordem de Serviço (OS)**: ID, número, data de emissão, data prevista de conclusão, status, valor total, veículo e equipe responsáveis  
6. **Serviço**: ID, descrição, valor de mão-de-obra  
7. **Peça**: ID, descrição, valor unitário  
8. **OS_Serviço**: Associação entre OS e Serviço (quantidade e valor calculado)  
9. **OS_Peça**: Associação entre OS e Peça (quantidade e valor total)  

---

## Observações
- O modelo permite **consultar histórico de serviços**, calcular valores e controlar equipes.  
- Permite também expandir funcionalidades, como **controle de estoque de peças** e **agendamento de revisões**.  

---

## Autor
Breno Rodrigues Bittencourt  



