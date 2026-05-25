# 📘 Fundamentos e Estruturas da Gestão Global de Segurança Cibernética

Projeto prático desenvolvido para explorar o uso da Inteligência Artificial (NotebookLM) para Treinar e orientar sobre CyberSegurança.

## 🎯 Contexto e Objetivos
- **Tema Escolhido:** Segurança Cibernética e Proteção aos usuários.
- **Objetivos de Estudo:**  Compreender como centralizar e analisar dados de segurança, entender o funcionamento de alertas e criar uma base teórica sólida.

## 📚 Curadoria de Fontes
Para alimentar o NotebookLM com informações precisas, as seguintes fontes abertas foram selecionadas e feito o upload:
1. Global Threat Intelligence Report - (https://irp.cdn-website.com/711a67a7/files/uploaded/Flashpoint_2026_Global_Threat_Intelligence_Report.pdf)]
2.  Norton Blog - (https://us.norton.com/blog?utm_source=chatgpt.com)
3. Kaspersky - (https://www.kaspersky.com.br/?utm_source=chatgpt.com)
4.  UMA ANÁLISE PRÁTICA DAS PRINCIPAIS VULNERABILIDADES EM
APLICAÇÕES WEB BASEADO NO TOP 10 OWASP UFCCQ, Felipe Ferreira Sampaio - https://repositorio.ufc.br/bitstream/riufc/62466/1/2021_tcc_ffsampaio.pdf
5.Securityu on the web / MDN - https://developer.mozilla.org/en-US/docs/Web/Security?utm_source=chatgpt.com
6. A arte de enganar Kevin D. Mitnick & William L. Simon - https://www.mariscotron.libertar.org/wp-content/uploads/2021/01/A-Arte-de-Enganar-%E2%80%93-Kevin-D.-Mitnick.pdf
7. OWSP security testing guide - https://owasp.org/www-project-web-security-testing-guide/
8. Malware Analysis and Reverse-Engineering Cheat Sheet - https://zeltser.com/media/docs/malware-analysis-cheat-sheet.pdf
9.  FEBRABAN TECH - segurnaça - https://febrabantech.febraban.org.br/temas/seguranca?utm_source=chatgpt.com
10. Introdução aos testes de Intrusão(Pentest) Leonardo Dias - https://semanacap.bcp.nic.br/files/apresentacao/arquivo/2147/Slides%20-%20Introdu%C3%A7%C3%A3o%20aos%20Testes%20de%20Intrus%C3%A3o%20(Pentest).pdf

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)
Durante a interação com a IA, testei diferentes abordagens para extrair as melhores respostas. Abaixo documento o raciocínio e os refinamentos:

- **Tentativa 1 (Prompt Inicial):** *"Discuss what these sources say about Prevenção de Engenharia Social, in the larger context of Controle do Fator Humano."*
  - **Resultado:** A prevenção da engenharia social no contexto do controle do fator humano baseia-se na premissa de que as pessoas são o elo mais fraco da segurança cibernética
. Mesmo organizações com tecnologias de defesa sofisticadas permanecem vulneráveis, pois os atacantes frequentemente optam pela "exploração do elemento humano" como o caminho de menor resistência para contornar proteções técnicas
.
A seguir, são detalhados os pilares desse controle e prevenção conforme as fontes:
1. Compreensão da Psicologia do Ataque
A engenharia social utiliza influência e persuasão para manipular indivíduos a realizarem ações ou revelarem informações confidenciais
. Para controlar o fator humano, é essencial entender os gatilhos psicológicos (Baseados nos princípios de Robert Cialdini) que os atacantes exploram
:
Autoridade: Tendência de atender solicitações de quem aparenta ter poder ou cargo elevado
.
Afabilidade (ou Liking): Atacantes simulam interesses comuns para criar afinidade e ganhar confiança
.
Reciprocidade: Oferecer um favor (como "ajuda" técnica) para que a vítima se sinta obrigada a retribuir
.
Consistência: Após um pequeno compromisso público, o indivíduo tende a seguir instruções para parecer coerente
.
Validação Social: Agir conforme o que os outros parecem estar fazendo no ambiente corporativo
.
Escassez: Criar senso de urgência para forçar uma decisão rápida e sem análise
.
2. Treinamento e Conscientização Contínua
A única defesa efetiva contra a fraude humana é educar e treinar o pessoal para identificar o engenheiro social
.
Programas Dinâmicos: O treinamento deve ser interessante e interativo, utilizando dramatização e simulações (como de phishing e pretexting) para demonstrar as táticas na prática
.
Conscientização Específica: Diferentes grupos (gerentes, TI, recepcionistas, guardas) precisam de orientações adaptadas às suas funções, já que todos podem ser alvos
.
Cultura de Vigilância: É necessário motivar os funcionários a aceitarem a segurança como parte de seu trabalho, incentivando o desafio educado a estranhos ou solicitações incomuns
.
3. Implementação de Políticas e Procedimentos
O controle do fator humano requer regras claras que retirem a subjetividade da tomada de decisão dos funcionários
.
Classificação de Dados: Estabelecer níveis de confidencialidade (Interno, Particular, Confidencial) para que o empregado saiba exatamente o que pode ou não ser compartilhado e com quem
.
Protocolos de Verificação: Nenhuma informação deve ser liberada sem a verificação positiva da identidade do solicitante
. Isso inclui ligar de volta para números oficiais do diretório da empresa e não confiar cegamente no identificador de chamadas, que pode ser forjado
.
Ponto Central de Relato: Instituir um local único para relatar incidentes suspeitos, permitindo que a empresa detecte ataques coordenados em andamento e alerte os demais funcionários
.
4. Controles Técnicos Complementares
Embora o foco seja humano, a tecnologia deve ser usada para reforçar a "firewall humana"
:
Autenticação Multifator (MFA): Embora Mitnick advirta que atacantes astutos podem tentar contornar tokens, o uso de MFA (incluindo biometria) dificulta o roubo de contas apenas por credenciais obtidas via engenharia social
.
SAST e Higiene de Segurança: O uso de ferramentas de análise estática de código cedo no desenvolvimento educa os times sobre boas práticas e reduz vulnerabilidades exploráveis
.
Gestão de Identidade (IAM): Implementar o princípio do menor privilégio garante que, mesmo que uma conta seja comprometida por engenharia social, o dano seja limitado
.
Em resumo, o controle do fator humano não busca tornar os funcionários paranoicos, mas sim transformá-los de alvos vulneráveis em uma linha de defesa ativa, fundamentada no lema: "Verifique, verifique, verifique"
  
  
- **Tentativa 2 (Prompt Refinado):** *"Atuando como um analista SOC, explique com base nos documentos anexados como o [Conceito X] ajuda na detecção de ameaças."*
  - **Resultado:** Resposta excelente e embasada, conectando a teoria com a prática defensiva.
    📖 Glossário
Engenharia Social: Tática cibernética que utiliza manipulação psicológica, persuasão e influência para induzir indivíduos a realizarem ações inseguras ou revelarem informações confidenciais, contornando proteções tecnológicas.

Firewall Humana: Conceito defensivo que visa transformar os colaboradores de uma organização — frequentemente vistos como o elo mais fraco — em uma linha de defesa ativa e vigilante por meio de treinamento contínuo e cultura de verificação.

Gatilhos Psicológicos: Princípios de comportamento humano (como Autoridade, Escassez, Reciprocidade e Validação Social) explorados por atacantes para criar senso de urgência, afinidade ou medo, forçando a vítima a agir sem análise crítica.

Pretexting: Técnica específica de engenharia social onde o invasor cria um cenário fictício detalhado (pretexto), muitas vezes assumindo uma falsa identidade, para justificar a solicitação de dados sensíveis.

Princípio do Menor Privilégio: Regra de Governança e Gestão de Identidade (IAM) que garante que cada usuário ou sistema tenha apenas o nível mínimo de acesso necessário para realizar suas funções, limitando o raio de explosão (dano) caso uma conta seja comprometida.
🔁 Prompts Reutilizáveis
Para revisar este material no futuro, os seguintes prompts podem ser utilizados em qualquer IA:

"Gere um quiz de 5 perguntas de múltipla escolha sobre Prevenção de Engenharia Social e Gatilhos Psicológicos corporativos, focando no nível de dificuldade intermediário para analistas de SOC."

"Aja como um recrutador técnico de Cibersegurança e me faça uma pergunta situacional de entrevista sobre como eu ajudaria a implementar controles do fator humano e mitigar ataques de phishing em uma empresa de grande porte."
