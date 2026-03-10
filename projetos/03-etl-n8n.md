\# ⚡ ETL Industrial com n8n



\## Link Principal

🔗 \[github.com/Ronan-Rodrigues/etl-industrial-n8n](https://github.com/Ronan-Rodrigues/etl-industrial-n8n)



\## Conceito

Coleção de workflows de automação de processos industriais usando n8n,

replicando em software moderno o que fazia com supervisórios Elipse E3

e macros VBA Excel.



\## Workflows Incluídos



\### 1. 🔥 Alerta de Temperatura Crítica

\*\*Cenário:\*\* Monitoramento de chillers e estufas (experiência LFDA)



\*\*Lógica:\*\*

IF temperatura > limite\_max OR temperatura < limite\_min

THEN enviar\_alertas() AND registrar\_evento() AND escalar\_se\_nao\_confirmado(10min)





\*\*Canais:\*\* Email + WhatsApp + Telegram



---



\### 2. 📈 Relatório Diário Automático

\*\*Substitui:\*\* Macros VBA que desenvolvia em Excel



\*\*Schedule:\*\* Todo dia, 06:00



\*\*Processo:\*\*

1\. Query no banco (médias, máximas, mínimas do dia anterior)

2\. Gera Excel formatado

3\. Converte para PDF

4\. Envia por email para gestores

5\. Atualiza dashboard Power BI



---



\### 3. 🔧 Ordem de Manutenção Preventiva

\*\*Cenário:\*\* Controle de PM na Globo Pharma



\*\*Trigger:\*\* Baseado em horímetro, contador de ciclos ou tempo calendário



\*\*Ações:\*\*

\- Cria card no Trello/Notion

\- Notifica técnico responsável (WhatsApp)

\- Agenda no calendário Google

\- Escalada se não executada em prazo



---



\### 4. 📊 Integração Power BI

\*\*Push de dados\*\* para datasets do Power BI via API a cada 15 minutos



---



\### 5. 🔄 Backup e Arquivamento

\*\*Rotina noturna:\*\*

\- Compacta logs do dia

\- Upload para AWS S3

\- Limpa registros antigos do banco

\- Confirmação por email



\## Stack Completo

| Componente | Tecnologia |

|-----------|-----------|

| Orquestração | n8n |

| Banco de Dados | PostgreSQL / MySQL |

| Planilhas | Google Sheets |

| BI | Power BI |

| Storage | AWS S3 |

| Comunicação | Webhooks, REST APIs |

| Notificações | Telegram, WhatsApp, Email |



\## Status

✅ \*\*Concluído e documentado\*\*

