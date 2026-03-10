\# 🤖 Chatbot PLC Controller com IA



\## Link Principal

🔗 \[github.com/Ronan-Rodrigues/chatbot-plc-controller](https://github.com/Ronan-Rodrigues/chatbot-plc-controller)



\## Conceito

Assistente virtual que interpreta comandos em linguagem natural e aciona 

saídas digitais em ESP32/Arduino — simulando controle de CLPs via conversa.



\## Stack Completo

| Camada | Tecnologia |

|--------|-----------|

| NLP/IA | Python + LangChain + OpenAI GPT-3.5 |

| Backend | Flask |

| Hardware | ESP32 + MicroPython |

| Comunicação | HTTP REST |

| Cache | Redis |

| Interface | Telegram Bot |

| Banco | PostgreSQL |



\## Funcionalidades Principais

\- \[x] Interpretação de comandos em português

\- \[x] Integração com LLM para entender variações de linguagem

\- \[x] Controle físico de relés/LEDs via ESP32

\- \[x] Feedback visual no hardware

\- \[x] Histórico de comandos em PostgreSQL

\- \[x] Interface Telegram para controle remoto



\## Exemplos de Comandos

| Comando do Usuário | Ação do Sistema |

|-------------------|-----------------|

| "Liga a luz da sala" | Aciona GPIO 12 |

| "Desligar tudo" | Desliga todas saídas |

| "Qual o status?" | Retorna estado de todas entradas |

| "Ligar ventilação se temperatura \&gt; 28" | Cria regra condicional |



\## Segurança Implementada

\- Autenticação por token no Telegram

\- Rate limiting (evita spam)

\- Confirmação de estado após execução

\- Logs de auditoria completos



\## Status

✅ \*\*Concluído e documentado\*\*

