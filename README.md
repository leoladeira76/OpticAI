# OpticAI
Ferramenta inteligente para análise e combate ao vandalismo, garantindo a segurança da rede com inteligência artificial. Análise preditiva e resposta a incidentes em redes de fibra óptica.

Analisador Inteligente de Relatos de Vandalismo em Redes de Fibra Óptica
Imersão IA 2025 - Alura & Google

Desafio
O vandalismo em redes de fibra óptica causa interrupções de serviço, prejuízos financeiros e coloca em risco a segurança da população. A análise eficiente dos relatos de incidentes é fundamental para uma resposta rápida e eficaz.

Solução Proposta
Este projeto utiliza a API do Gemini para criar um sistema inteligente que:
Analisa relatos de vandalismo em linguagem natural, extraindo informações cruciais como localização, tipo de dano, causa provável, recorrência e gravidade.
Classifica a gravidade do incidente para priorizar ações de resposta.
Identifica padrões em relatos recentes para auxiliar na investigação de possíveis ações coordenadas de vandalismo.

Funcionalidades
Análise de Relatos: O sistema processa relatos textuais de vandalismo, fornecendo uma análise estruturada do incidente.
Classificação de Gravidade: Os incidentes são classificados como Alta, Média ou Baixa gravidade, permitindo uma resposta mais eficiente.
Identificação de Padrões: O sistema busca padrões em múltiplos relatos, auxiliando na identificação de possíveis ações coordenadas.

Como Funciona
Entrada de Dados: Técnicos de campo ou o COP (centro de operações) inserem relatos de incidentes em linguagem natural.
Processamento com Gemini: O sistema utiliza a API do Gemini para analisar o texto do relato, extraindo informações relevantes e classificando a gravidade.
Análise de Padrões: O sistema compara os relatos recentes para identificar possíveis padrões.
Saída: O sistema gera um relatório estruturado com a análise do incidente, a classificação da gravidade e a identificação de padrões (se houver).


Arquitetura do Sistema

Tecnologias Utilizadas
Python, Google Gemini API e Google Colab (para desenvolvimento e execução)

Código
O código do projeto está estruturado em funções para facilitar a manutenção e a reutilização:
inicializar_api(): Inicializa a API do Gemini com a chave de API do usuário.
obter_modelos(): Lista os modelos disponíveis e retorna o nome do modelo utilizado.
criar_chat(): Cria uma sessão de chat com o modelo especificado e instrução de sistema.
analisar_relato(): Envia um relato de vandalismo para o chat e retorna a análise gerada pelo modelo.
extrair_informacoes_relato(): Extrai informações relevantes de um relato de vandalismo usando o Gemini.
classificar_gravidade(): Classifica a gravidade de um relato de vandalismo usando o Gemini.
identificar_padroes(): Tenta identificar padrões em relatos de vandalismo recentes.
main(): Função principal para executar o sistema de análise de relatos de vandalismo.

Exemplos de Uso
Entrada
Cabo rompido na Rua X, poste Y, suspeita de vandalismo com corte intencional, terceiro incidente na semana nesta região.

Saída
Localização: Rua X, poste Y
Tipo de Dano: Cabo Rompido
Causa Provável: Corte Intencional
Recorrência: Terceiro incidente na semana nesta região
Gravidade: Alta

Próximos Passos
Implementar um banco de dados para armazenar os relatos e facilitar a análise de padrões em larga escala.
Criar uma interface web para facilitar a entrada de dados e a visualização dos resultados.
Integrar este código com sistemas de gestão de incidentes existentes.
Desenvolver um modelo de machine learning para prever a ocorrência de vandalismo em determinadas áreas.

Conclusão
Este projeto demonstra o potencial da IA para auxiliar no combate ao vandalismo em redes de fibra óptica, permitindo uma resposta mais rápida e eficaz aos incidentes. Acreditamos que esta solução pode trazer benefícios significativos para o setor de telecomunicações, contribuindo para a segurança da infraestrutura e a qualidade dos serviços prestados à população.
