## 2.1 Base de Dados

Foi utilizada a base **INFLUD24-26-06-2025.csv**, disponibilizada pelo Ministério da Saúde por meio do portal *dados.gov.br*.  
A base contém **194 variáveis** relacionadas a notificações de SRAG, incluindo dados demográficos, clínicos, laboratoriais, evolução e localização.

---

## 2.2 Variáveis Utilizadas

Para a análise, foram selecionadas:

- **SG_UF_NOT** – Estado da notificação  
- **DT_NOTIFIC** – Data da notificação  
- **SEM_NOT** – Semana epidemiológica da notificação  
- **NU_NOTIFIC** – Número da notificação *(não usado analiticamente)*

---

## 2.3 Processamento e Limpeza

As seguintes etapas foram realizadas:

1. **Filtragem** dos registros em que `SG_UF_NOT == "MG"`.  
2. **Conversão** da coluna `DT_NOTIFIC` para formato de data.  
3. **Seleção** apenas de notificações do ano de **2024**.  
4. **Agrupamento** dos dados por semana epidemiológica (`SEM_NOT`).  

---

## 2.4 Ferramentas Utilizadas

- **Python + Pandas** para limpeza e agregações.  
- **Matplotlib** para geração dos gráficos.  
- **Ambiente:** ChatGPT Python Sandbox.
