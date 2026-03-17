# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 16 de Março de 2026  
**Empresa:** Abstergo Industries - Divisão Farmacêutica  
**Responsável:** Gabriel Demetrios Lafis

---

## Introdução

Este relatório apresenta o processo de implementação de ferramentas AWS na empresa Abstergo Industries (Divisão Farmacêutica), realizado por Gabriel Demetrios Lafis. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar diminuição de custos imediatos na operação farmacêutica da empresa.

## Descrição do Projeto

O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

### Etapa 1: Amazon S3 (Simple Storage Service)

- **Nome da ferramenta:** Amazon S3
- **Foco da ferramenta:** Armazenamento de objetos escalável e de baixo custo
- **Descrição de caso de uso:** Migração do sistema de armazenamento de documentos regulatórios, laudos laboratoriais, notas fiscais eletrônicas e registros de controle de qualidade da farmácia para o Amazon S3. Utilizando as classes de armazenamento S3 Intelligent-Tiering, os documentos acessados com menor frequência são automaticamente movidos para camadas de menor custo, reduzindo os gastos com armazenamento em até 40%. Além disso, a configuração de políticas de ciclo de vida permite que documentos com mais de 5 anos sejam arquivados no S3 Glacier Deep Archive, reduzindo ainda mais os custos de retenção obrigatória exigidos pela ANVISA.

### Etapa 2: Amazon EC2 Auto Scaling com Elastic Load Balancing

- **Nome da ferramenta:** Amazon EC2 Auto Scaling + Elastic Load Balancing
- **Foco da ferramenta:** Computação elástica e distribuição de carga
- **Descrição de caso de uso:** Implementação de Auto Scaling para o sistema de e-commerce farmacêutico e o sistema de gestão de estoque (ERP). Durante horários de pico (08h-12h e 18h-22h), o sistema escala horizontalmente para atender a demanda. Nos períodos de baixa utilização (madrugada e fins de semana), as instâncias são automaticamente reduzidas. Com o Elastic Load Balancing distribuindo o tráfego entre as instâncias, a empresa eliminou a necessidade de manter servidores superdimensionados 24/7, resultando em uma economia estimada de 35% nos custos de computação.

### Etapa 3: Amazon RDS (Relational Database Service)

- **Nome da ferramenta:** Amazon RDS
- **Foco da ferramenta:** Banco de dados relacional gerenciado
- **Descrição de caso de uso:** Migração do banco de dados de controle de medicamentos, prescrições e inventário farmacêutico para o Amazon RDS com engine PostgreSQL. O serviço gerenciado elimina a necessidade de uma equipe dedicada para administração de banco de dados (patches, backups, failover), reduzindo custos operacionais com pessoal de TI. A utilização de instâncias reservadas (Reserved Instances) com compromisso de 1 ano proporciona desconto de até 40% em relação ao modelo sob demanda. O recurso de Multi-AZ garante alta disponibilidade para dados críticos de saúde sem custos adicionais significativos.

## Conclusão

A implementação de ferramentas na empresa Abstergo Industries - Divisão Farmacêutica tem como esperado a redução de custos operacionais em infraestrutura de TI, o aumento da eficiência no gerenciamento de dados farmacêuticos e a melhoria na escalabilidade dos sistemas. A economia total estimada com as três etapas é de aproximadamente 35-45% nos custos de infraestrutura, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa, como a adoção futura do Amazon DynamoDB para dados de IoT de monitoramento de temperatura de medicamentos e o AWS Lambda para processamento serverless de eventos.

## Anexos

- [Documentação Amazon S3](https://aws.amazon.com/s3/)
- [Documentação Amazon EC2 Auto Scaling](https://aws.amazon.com/ec2/autoscaling/)
- [Documentação Amazon RDS](https://aws.amazon.com/rds/)
- [AWS Well-Architected Framework - Cost Optimization Pillar](https://aws.amazon.com/architecture/well-architected/)
- [AWS Pricing Calculator](https://calculator.aws/)

---

**Assinatura do Responsável pelo Projeto:**

Gabriel Demetrios Lafis

---

## 🛠️ Tecnologias Utilizadas

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)

## 📋 Licença

Este projeto está sob a licença MIT.
