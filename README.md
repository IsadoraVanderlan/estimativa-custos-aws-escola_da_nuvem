# 🚀 Estimativa de Custos AWS: Aplicação Web de Três Camadas

> **Projeto prático desenvolvido durante o treinamento da Escola da Nuvem.**

## 📌 Visão Geral
Este repositório documenta o processo de análise financeira e técnica para a implementação de uma infraestrutura na nuvem AWS. Utilizando a **AWS Pricing Calculator**, foi elaborada uma estimativa detalhada para uma aplicação web resiliente e escalável.

## 🏗️ Arquitetura e Fluxo do Lab
Para este estudo de caso, projetei o seguinte fluxo de trabalho e componentes:

![Fluxo do Processo](./diagrama.jpg)

### Componentes Estimados:

*   **Load Balancer (ALB):**
    *   Configurado para 400 requisições/seg e 100 novas conexões/seg.
    *   20 avaliações de regra por solicitação.
*   **Amazon EC2 (Camada de Aplicação):**
    *   Instâncias **t4g.small** (Processadores AWS Graviton).
    *   Escalabilidade dinâmica: 1 instância (Base) / 2 instâncias (Pico).
    *   Armazenamento: 30 GB SSD (gp3).
    *   Tráfego de saída: 200 GB/mês.
*   **Amazon RDS (Camada de Dados):**
    *   Motor MySQL com instância **db.m6g.large**.
    *   Implantação **Multi-AZ** para alta disponibilidade.
    *   Armazenamento: 100 GB SSD (gp2).

## 🛠️ Ferramentas Utilizadas
*   **AWS Pricing Calculator**: Modelagem de custos.
*   **Diagramação**: Criação de fluxo visual personalizado.
*   **Região**: US West (Oregon).

## 📈 Conclusões do Projeto
O laboratório permitiu aplicar conceitos de **FinOps**, entendendo como a escolha de instâncias (Graviton) e modelos de implantação (Multi-AZ) impactam o custo total de propriedade (TCO). A estimativa final foi exportada em CSV para análise em planilhas e compartilhada via link público para stakeholders.

---
✨ *Projeto focado em Arquitetura de Soluções e Gestão de Custos em Nuvem.*
