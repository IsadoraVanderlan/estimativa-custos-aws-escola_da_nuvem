# 🎓 Projeto Final: Operações em Nuvem (AWS Educate)

Este repositório contém o projeto final de conclusão do curso **Operações em Nuvem** da plataforma **AWS Educate**. O desafio consistiu em arquitetar e estimar os custos de uma solução escalável e de alta disponibilidade na AWS.

## 🎯 Objetivo do Projeto
Demonstrar proficiência no uso da **AWS Pricing Calculator** para planejar o custo total de propriedade (TCO) de uma aplicação web de três camadas, aplicando conceitos de escalabilidade, alta disponibilidade e otimização de custos (FinOps).

## 📊 Arquitetura Estimada & Fluxo
Abaixo, apresento o diagrama que desenvolvi para ilustrar o fluxo:

![Diagrama de Fluxo](./diagrama_animado.svg)

### Detalhes da Infraestrutura (Região Oregon):
*   **Networking:** 1 Application Load Balancer (ALB) para gestão de tráfego (400 req/s).
*   **Computação (EC2):** Instâncias **t4g.small** (Linux) com modelo de escalabilidade para picos de demanda.
*   **Banco de Dados (RDS):** MySQL em **Multi-AZ** (db.m6g.large) para garantir resiliência e failover automático.
*   **Armazenamento e Tráfego:** Configuração de volumes EBS gp3, armazenamento RDS gp2 e 200GB de saída de dados (Data Transfer Out).

## 🛠️ Competências Desenvolvidas
*   **Análise de Custos:** Modelagem financeira detalhada de serviços de nuvem.
*   **Design de Arquitetura:** Seleção de instâncias e estratégias de implantação baseadas em requisitos de carga.
*   **Documentação Técnica:** Elaboração de diagramas de fluxo e exportação de relatórios (CSV) para suporte à decisão.


---
🚀 *Projeto finalizado com sucesso como parte da trilha de aprendizado em Cloud Computing.*
