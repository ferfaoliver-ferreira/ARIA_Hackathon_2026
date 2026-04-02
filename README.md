**ARIA: Análise Regulatória com Inteligência Artificial Vencedor do Case: "GenAI para extrair conhecimento de dados complexos"**  

**🥈VENCEDOR DO SEGUNDO LUGAR no Hackathon Talento Tech 3.0 Hacking for Good (2026).**


**🌟 Visão Geral**

A **ARIA** (Análise Regulatória com Inteligência Artificial) é uma plataforma de Inteligência Regulatória baseada em **IA Generativa** que automatiza a ingestão, interpretação e monitoramento contínuo de documentos científicos e normas técnicas.

Desenvolvida durante o **Hackathon Talento Tech 3.0**, o projeto transforma bases de dados estáticas (PDFs de editais, dossiês e ensaios clínicos) em um "cérebro corporativo" vivo, consultável em linguagem natural e baseado em evidências.

Persona:

**"Hoje, a indústria farmacêutica precisa de automação na gestão de informações técnicas e regulatórias quando o alto volume de documentos complexos gera riscos de inconformidade e lentidão na tomada de decisão."** 

**Exemplo:**   

**Antes:** Renata gasta **15 horas por semana** lendo manualmente atualizações da Anvisa e novos ensaios clínicos de outras fontes para garantir que a empresa não sofra sanções.

**Depois (com ARIA):** **Todos os dias as 6 da manhã** a ARIA faz busca por novos documentos em sites oficiais (cadastrados na implementação).  
Renata, quando chega ao trabalho as 8 da manhã, recebe um alerta com um resumo executivo pronto, com o que mudou e o impacto nos produtos da empresa.


🚀**Diferenciais da Solução**   
Diferente de ferramentas de busca comuns, a **ARIA** utiliza:  

**1. RAG (Retrieval-Augmented Generation)**: Garante que as respostas da IA sejam baseadas estritamente nos documentos carregados, eliminando "alucinações" e fornecendo citações de fonte (página/parágrafo).

**2. Ingestão Proativa**: O sistema não é passivo. Ele utiliza o **Amazon EventBridge** para monitorar e baixar atualizações de órgãos reguladores (como ANVISA/FDA) de forma autônoma.  

**3. Extração Especializada**: Integração do **Amazon Textract** com **Comprehend Medical** para identificar dosagens, princípios ativos e relações clínicas complexas.

🛠️ **Arquitetura Técnica (AWS Cloud Native)**  

A solução foi desenhada sob o **AWS Well-Architected Framework**, garantindo escalabilidade e baixo custo:  

**- Camada de Ingestão**: AWS API Gateway + S3 (com políticas de Lifecycle e Object Lock para integridade regulatória).  

**- Orquestração: AWS Step Functions** gerencia o fluxo de processamento, garantindo que falhas sejam tratadas via filas de mensagens (Amazon SQS).  

**- Cérebro de IA: Amazon Bedrock** (utilizando modelos como Claude 3 Haiku para velocidade e custo) integrado ao **Amazon OpenSearch Serverless** para busca vetorial.  

**- Segurança:** Implementação de **AWS WAF** para proteção de borda e criptografia de dados em repouso e em trânsito.

**- Monitoramento:** 24/7


**Vídeo Demonstração**    


[Projeto-Aria-hachaton - Copia.webm](https://github.com/user-attachments/assets/9f3c8283-5d8f-49ef-9b2c-5cc480f20a1d)  





📊 **Impacto e Métricas de Sucesso:**
<img width="1958" height="817" alt="métricas para slide recorte" src="https://github.com/user-attachments/assets/ec37040b-32e8-4b1e-93d8-d6dedc0d2765" />

🧪 **Validação e Prova de Conceito (PoC)**  

O sistema foi validado com documentos reais, demonstrando a capacidade de extrair "insights" de textos densos e gerar respostas estruturadas

![testes ARIA](https://github.com/user-attachments/assets/051fa2ae-43ac-4d0c-b8b6-4d75c801b6db)




💰 **FinOps e Viabilidade Econômica:**

O projeto foi submetido a uma estimativa rigorosa na **AWS Pricing Calculator:**
**- Custo Mensal Estimado:** $305,18.
**- Otimização de Custo:** O componente mais caro é o OpenSearch ($263,04). Para empresas menores, propomos o **Roadmap de Redução** substituindo-o por **RDS com pgvector**, reduzindo o custo mensal para aproximadamente **$57,00**.
**- Governança:** Configuração de **AWS Budgets** com alarmes em 60% do orçamento previsto.


🌿 **Sustentabilidade (ESG - Hacking for Good)**  
A ARIA promove a **Desmaterialização** e a **Eficiência Energética:**
- Redução de Resíduos: Eliminação física de milhares de páginas de papel no fluxo regulatório.
- Serverless First: O uso de **AWS Lambda** garante que a computação ocorra apenas sob demanda, minimizando o desperdício energético em comparação com servidores legados ligados 24/7.

  <img width="654" height="186" alt="impacto ambiental image" src="https://github.com/user-attachments/assets/3f7f346a-9f6b-4031-84bb-86f2c1e051e7" />

🆙**Próximos Passos e Melhorias Futuras**  
**Roadmap**

**Semana 1:** Segurança e Gestão de identidade - Implementação do **Amazon Cognito**

**Semana 2:** FinOps e Prevenção de Custos – Cache Semântico (uma opção é o **DynamoDB**)

**Avaliação contínua:** Avaliação de Qualidade da IA - Comparar a taxa de precisão x custo por token gerado


🤝**Projeto vencedor do segundo lugar desenvolvido por:**  

**- Fernanda Ferreira de Oliveira**  
**- Gustavo Dias**  
**- Melina Nascimento França**  
**- Tadeu Silva de Queiroz**  
**- Vinicio Rocha dos Reis**  

![WhatsApp Image 2026-04-01 at 21 43 13](https://github.com/user-attachments/assets/77302566-d392-4ea1-bf14-fd2128c24b03)

🏢 Realização e Apoio:
Este projeto foi fruto do **Hackathon Talento Tech 3.0**, apresentado no **SENAI Santo Amaro (Suíço-Brasileira)**.

**Parceiros:**  
**- Escola da Nuvem**  
**-  AWS**  
**- TD SYNNEX**  
**- Dedalus**  
**- BRLink**  
**- Enkel**  
**- Darede**  
