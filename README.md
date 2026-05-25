# FATEC CI/CD - Pipeline de Integração Contínua e Entrega Contínua

Sobre o Projeto

Este projeto foi criado como parte de uma atividade acadêmica da FATEC, com a finalidade de aplicar conceitos de Integração e Entrega Contínua (CI/CD) utilizando GitHub Actions.
Além da automação da pipeline, o trabalho também explorou o uso do CodeQL para análise estática de segurança em aplicações Python, permitindo identificar possíveis vulnerabilidades durante o processo de desenvolvimento e testes automatizados.
O objetivo principal foi compreender na prática como ferramentas de DevOps e segurança podem atuar juntas para aumentar a qualidade e a confiabilidade do software.



🛠️ Tecnologias Utilizadas
TecnologiaFinalidadeGitHubArmazenamento do projeto e controle de versõesGitHub ActionsExecução automatizada da pipeline CI/CDCodeQLVerificação de vulnerabilidades e análise de segurançaPythonDesenvolvimento da aplicação utilizada nos testes



⚙️ Objetivo da Pipeline

A pipeline foi estruturada para automatizar etapas importantes do desenvolvimento, garantindo mais qualidade e segurança no projeto. Entre os principais objetivos estão:

✅ Executar testes automaticamente a cada atualização do código
🔍 Realizar verificações de segurança de forma contínua
🚨 Identificar possíveis vulnerabilidades na aplicação Python
📐 Incentivar o uso de boas práticas no desenvolvimento seguro
🧪 Demonstrar, na prática, a integração do CodeQL em um fluxo CI/CD real


🔄 Fluxo da Pipeline
Sempre que um código é enviado para o GitHub, a pipeline é iniciada automaticamente pelo GitHub Actions.
Depois disso, o sistema instala as dependências necessárias do projeto e executa os testes automatizados para verificar se tudo está funcionando corretamente.
Na sequência, o CodeQL realiza uma análise de segurança no código-fonte, buscando possíveis vulnerabilidades e falhas conhecidas.
Por fim, a pipeline retorna o resultado: caso esteja tudo certo, ela é aprovada; se algum erro ou vulnerabilidade for encontrado, o processo é bloqueado para evitar problemas na aplicação.


🧪 Cenários Testados
✅ Teste 1 — Código Seguro
Foi utilizado um código Python sem vulnerabilidades conhecidas, seguindo boas práticas de desenvolvimento e segurança.
Resultado obtido: a pipeline foi executada com sucesso, todos os testes passaram corretamente e o CodeQL não identificou falhas de segurança na aplicação.
📷 Evidência: print da pipeline com todos os jobs em verde no GitHub Actions.


<img width="1872" height="862" alt="image" src="https://github.com/user-attachments/assets/d860a028-44ea-4cfa-9604-6a72c0fba356" />


❌ Teste 2 — Código Vulnerável
Inserção proposital de vulnerabilidade SQL Injection (CWE-89):

<img width="1908" height="886" alt="image" src="https://github.com/user-attachments/assets/8a96bad7-d820-4239-94ab-47ba4c472aa9" />


🔒 Teste 3 — Código Corrigido
Correção aplicada com consultas parametrizadas.

📷 Evidência:

<img width="1894" height="887" alt="image" src="https://github.com/user-attachments/assets/24f9d7f7-b856-43be-bafa-c305b9bfaa6f" />



🔍 Outras Vulnerabilidades Estudadas
CWE	Tipo
CWE-78	Command Injection
CWE-22	Path Traversal
CWE-798	Hard-coded Credentials
CWE-327	Weak Cryptography
CWE-502	Insecure Deserialization
CWE-94	Uso inseguro de eval()
CWE-338	Geração insegura de números aleatórios



📚 Aprendizados Obtidos
🔁 Funcionamento de uma pipeline CI/CD
🤖 Automação de verificações de segurança
🔬 Importância da análise estática de código
🛡️ Detecção de vulnerabilidades com CodeQL
📖 Boas práticas de desenvolvimento seguro
🔗 Integração entre GitHub Actions e CodeQL



✅ Conclusão
Este projeto permitiu compreender, na prática, a importância da integração entre automação, testes e segurança no processo de desenvolvimento de software.
A implementação da pipeline CI/CD com GitHub Actions possibilitou a execução automática de testes e validações a cada alteração realizada no código. Além disso, o uso do CodeQL demonstrou como vulnerabilidades podem ser identificadas antecipadamente, aumentando a confiabilidade e a proteção da aplicação.
Dessa forma, o trabalho evidenciou a aplicação de conceitos de DevSecOps, reforçando a adoção de práticas de desenvolvimento mais seguras, organizadas e eficientes.



👨‍💻 Autor
Projeto desenvolvido para fins acadêmicos na FATEC.














