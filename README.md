🛡️ Guia de Terminal & Shell para Cibersegurança com NotebookLM

Este repositório contém o projeto final do desafio da DIO, onde utilizei a inteligência artificial NotebookLM para criar um "Segundo Cérebro" focado em operações de Red Team, enumeração de redes e escalação de privilégios em ambientes Linux e Windows.
🎯 Contexto e Objetivos

No cenário de Cibersegurança, a velocidade e a precisão no uso do terminal são decisivas. Este projeto visa consolidar conhecimentos dispersos em manuais técnicos em uma base de conhecimento interativa e de consulta rápida.

Objetivos de Estudo:

    Domínio de CLI: Sistematizar comandos de PowerShell e Bash para automação de tarefas.

    Metodologias de Ataque: Compreender o encadeamento de ferramentas (Nmap + Metasploit + Shell).

    Escalação de Privilégios: Identificar vetores de ataque em Active Directory e sistemas Linux.

📚 Curadoria de Fontes

Para alimentar o NotebookLM, selecionei fontes técnicas de alta densidade:

    Briefing Document (Advanced Network Enumeration): Documento síntese sobre metodologias de Active Directory e NSE.

    Cybersecurity Bash Essentials: Guia de comandos fundamentais de Linux para segurança.

    PowerShell for Privilege Escalation: Manual focado em táticas de "Living-off-the-land" (LotL).

    Tcpdump & Nmap Scripting (NSE): Documentação técnica sobre análise de pacotes e automação de varreduras.

    Hashcat & John the Ripper Manuals: Referências para quebra de hashes e pós-exploração.

🧠 Engenharia de Prompts e "Cicatrizes"

Abaixo, descrevo os testes realizados para extrair o melhor da IA e as dificuldades encontradas.
Prompts Estratégicos:

    Prompt de Correlação: "Com base no relatório de Network Enumeration, crie uma tabela comparativa entre comandos de reconhecimento no Windows (CMD) e seus equivalentes no Linux (Bash)."

    Prompt de Automação: "Gere um script one-liner em Bash que filtre logs de saída do Nmap buscando por vulnerabilidades críticas (CVEs)."

    Prompt de Defesa (Blue Team): "Quais são os Event IDs do Windows gerados quando o comando Get-NetUser do PowerView é executado?"

Cicatrizes (Troubleshooting):

    Alucinação Técnica: Inicialmente, a IA misturou parâmetros do Nmap com ferramentas de brute-force.

    Correção: Refinei o prompt exigindo que a IA citasse a página ou a fonte específica do manual carregado, o que aumentou a fidelidade técnica em 90%.

    Formatação: Documentos em PDF com muitas imagens geravam ruído. Optei por converter partes críticas em Markdown/Texto para melhorar o processamento.

📖 Miniguia de Estudo
1. Resumo Estruturado: Metodologias de Ataque

    Fase 1: Reconhecimento: Uso do Nmap com categorias de scripts auth, discovery e vuln para mapear a superfície de ataque.

    Fase 2: Enumeração AD: Utilização do PowerShell (PowerView) para mapear GPOs, relações de confiança (Trusts) e encontrar senhas em campos de descrição de usuários.

    Fase 3: Escalação de Privilégios: Exploração de binários SUID no Linux e má configuração de permissões de ACL no Windows.

2. Glossário de Conceitos Chave
   
Termo	Definição

Living-off-the-land (LotL)	Uso de ferramentas nativas do sistema (como PowerShell) para realizar ataques, evitando detecção por antivírus.

NSE (Nmap Scripting Engine)	Sistema de scripts em Lua que estende as capacidades do Nmap para descoberta de vulnerabilidades.
Reverse Shell	Técnica onde a máquina alvo se conecta ao atacante, contornando firewalls que bloqueiam conexões de entrada.

GPO (Group Policy Object)	Configurações de segurança do Windows que, se mal aplicadas, podem permitir que usuários comuns virem administradores.

4. Prompts Reutilizáveis para Revisão

    "Resuma os 5 principais vetores de escalação de privilégios em Linux baseados nas minhas fontes."

    "Crie um checklist de comandos para enumeração inicial de um controlador de domínio."

Link para o NotebookLM: https://notebooklm.google.com/notebook/e86e6f68-8f11-4610-9114-d8092f4fa328

Projeto desenvolvido para Bootcamp de Cibersegurança da DIO
Autor: Pedro Henrique dos Santos
LinkedIn: www.linkedin.com/in/pedrohenriquedsantos
