# Plano Orçamentário -- Rede Industrial para Fábrica de Tijolo Ecológico

## 1. Levantamento Técnico do Processo

A indústria de tijolos ecológicos possui as seguintes etapas produtivas:

-   Reservatórios de água, cimento, areia e terra
-   Peneiragem
-   Dosagem dos materiais
-   Mistura manual ou betoneira
-   Prensagem
-   Cura

Objetivo: Implantar uma rede industrial com automação para controle de
produção, rastreabilidade e futura integração com sistemas corporativos
(ERP/MES).

------------------------------------------------------------------------

## 2. Infraestrutura Proposta (Resumo)

| Equipamentos | Descrição |
|---|---|
| CLP industrial | Comunicação Ethernet (Modbus TCP / Profinet) |
| IHM | Interface para operação local |
| Inversores de frequência | Controle de motores |
| Sensores | Nível, umidade e células de carga |
| Switch industrial | 8 portas |
| Cabeamento | Blindado (Ethernet e instrumentação) |
| Sistema supervisório | SCADA |
| Integração | Rede corporativa |

Investimento estimado: R\$ 21.500 a R\$ 25.000

------------------------------------------------------------------------

# 3. Análise de Viabilidade Técnica e Econômica

## 3.1 Viabilidade Técnica

A solução proposta é tecnicamente viável pois:

-   Utiliza equipamentos industriais consolidados no mercado.
-   Comunicação baseada em Ethernet industrial (Modbus TCP / Profinet).
-   Cabeamento blindado adequado para ambientes com poeira e
    interferência eletromagnética.
-   Instalação em painel elétrico com proteção adequada.

### Escalabilidade

-   CLP com possibilidade de expansão de módulos I/O.
-   Switch industrial permite inclusão de novos dispositivos.
-   Arquitetura preparada para integração futura com IoT industrial.
-   Possibilidade de adicionar novas prensas ou sensores sem alterar a
    estrutura principal.

### Compatibilidade com Sistemas Corporativos

-   Integração com ERP via banco de dados ou API.
-   Compatível com supervisórios SCADA.
-   Permite futura implementação de MES (Manufacturing Execution
    System).
-   Dados podem ser enviados para servidores corporativos ou nuvem.

------------------------------------------------------------------------

## 3.2 Análise Econômica

### Investimento Inicial

| Item | Valor |
|---|---|
| Investimento estimado | R\$ 21.500 a R\$ 25.000 |

### Benefícios Financeiros

-   Redução de desperdício de matéria-prima (estimativa 5% a 10%).
-   Padronização da qualidade dos tijolos.
-   Redução de retrabalho.
-   Maior controle de estoque.
-   Diminuição de falhas operacionais.

### Estimativa de Retorno do Investimento (ROI)

| Métrica | Valor |
|---|---|
| Economia média mensal | R\$ 3.000 a R\$ 4.000 |
| Investimento médio | R\$ 23.000 |
| Retorno estimado | 6 a 8 meses |

------------------------------------------------------------------------

## 3.3 Riscos Envolvidos

| Risco | Mitigação |
|---|---|
| Dependência de fornecedores específicos | Utilizar marcas consolidadas |
| Aumento do custo de manutenção especializada | Contrato de suporte técnico |
| Necessidade de treinamento dos operadores | Treinamento interno |
| Possíveis atrasos na entrega de equipamentos | Planejamento de estoque mínimo de peças críticas |

------------------------------------------------------------------------

## 3.4 Dependência de Fornecedores

| Componente | Fornecedor | Disponibilidade |
|---|---|---|
| CLP e IHM | Nacionais e importados | Alta |
| Inversores | Fabricante nacional | Local |
| Cabeamento | Múltiplos fornecedores | Ampla |

Risco considerado moderado, pois há múltiplos fornecedores disponíveis.

------------------------------------------------------------------------

# 4. Visualização Inicial da Arquitetura da Rede Industrial

## 4.1 Diagrama Conceitual da Arquitetura

Representação simplificada da solução:

```
                    ┌─────────────────────────┐
                    │     Rede Corporativa     │
                    │        (ERP/MES)         │
                    └────────────┬────────────┘
                                 │
                        ┌────────▼────────┐
                        │   Firewall /    │
                        │   Roteador      │
                        └────────┬────────┘
                                 │
                        ┌────────▼────────┐
                        │ Switch Industrial│
                        └─────┬────┬──────┘
                              │    │
                ┌─────────────┘    └─────────────┐
                │                                  │
        ┌───────▼───────┐                  ┌──────▼──────┐
        │      CLP      │                  │    IHM       │
        └───────┬───────┘                  └──────────────┘
                │
        ┌───────┼───────────────┬───────────────┐
        │       │               │               │
     Sensores  Células       Inversor        Inversor
    (nível/um) de carga   Betoneira         Prensa
```

------------------------------------------------------------------------

## 4.2 Expansão Futura

-   Inclusão de novos sensores na rede.
-   Implementação de monitoramento remoto.
-   Integração com banco de dados na nuvem.
-   Ampliação para múltiplas linhas de produção.

------------------------------------------------------------------------

## 5. Benefícios Estratégicos para o Negócio

-   Maior competitividade no mercado.
-   Controle em tempo real da produção.
-   Base tecnológica para crescimento da empresa.
-   Redução de custos operacionais.
-   Melhor tomada de decisão baseada em dados.

Observação: Caso desejado, o diagrama pode ser modelado no Cisco Packet
Tracer e inserido como imagem no relatório final para melhor
apresentação visual.

