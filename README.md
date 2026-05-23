# Nome do Grupo: LIORA

## Sobre o Projeto

O projeto desenvolvido pela Liora,  é uma solução desenvolvida para o Challenge 2026 da parceria entre a FIAP e a SPI Integração, com foco na transformação da segurança industrial tradicional em um modelo inteligente, preventivo e proativo dentro do conceito de **Metaindústria**.

A proposta utiliza Inteligência Artificial e Visão Computacional para monitorar continuamente o uso correto de Equipamentos de Proteção Individual (EPIs) em ambientes industriais, identificando riscos em tempo real e emitindo alertas preventivos antes que acidentes ocorram.

---

# Integrantes

* Bruno Takaya
* Iury Cardoso Araujo
* Kethely Ester da Silva
* Vanessa Iris Nobre Ribas 
* Raissa Yukari Senoi


---

# Problema Abordado

Muitas indústrias ainda utilizam um modelo de segurança baseado apenas em fiscalização punitiva, onde ações corretivas acontecem somente após falhas ou acidentes.

Os principais problemas encontrados são:

* Falta de monitoramento contínuo;
* Uso incorreto ou ausência de EPIs;
* Risco elevado de acidentes de trabalho;
* Dependência exclusiva de supervisão humana;
* Demora na identificação de situações perigosas;
* Falta de dados inteligentes para prevenção.

Dentro do contexto da Metaindústria, torna-se necessário um sistema automatizado capaz de atuar preventivamente e em tempo real.

---

# Proposta de Solução

Estamos propondo um sistema inteligente de monitoramento industrial baseado em Visão Computacional e Inteligência Artificial.

A solução realizará:

* Detecção automática de EPIs;
* Identificação de ausência de capacete, óculos, luvas, etc;
* Monitoramento contínuo em tempo real;
* Emissão de alertas imediatos;
* Registro de ocorrências;
* Dashboard para supervisão;
* Geração de relatórios preventivos.

O sistema busca criar uma cultura de prevenção, reduzindo acidentes e aumentando a segurança dos colaboradores.

---

# Público-Alvo

## Funcionário
Responsável pelas atividades operacionais da indústria.

## Administrador
Responsável pelo monitoramento dos colaboradores e análise de alertas.

---

# Diagramas UML

## Diagrama de Casos de Uso

![Diagrama de Casos de Uso](https://github.com/VanessaRibas/Sprint1---Engenharia-de-Software/tree/main/assets/Diagrama_de_Casos_de_Uso.jpg)

## Diagrama de Atividade

![Diagrama de Atividade](https://github.com/VanessaRibas/Sprint1---Engenharia-de-Software/tree/main/assets/Diagrama_de_Classes.drawio.png)


## Diagrama de Classes

![Diagrama de Classes](https://github.com/VanessaRibas/Sprint1---Engenharia-de-Software/tree/main/assets/Diagrama_de_Atividade.drawio.png)

---

# Tecnologias Selecionadas

| Tecnologia             | Finalidade                       |
| ---------------------- | -------------------------------- |
| Python                 | Desenvolvimento da IA e back-end |
| YOLOv8m                | Detecção de objetos e EPIs       |
| OpenCV                 | Processamento de imagens         |
| MySQL                  | Banco de dados                   |
| React Native           | Interface web                    |

---

# Justificativa Técnica

## Python

Escolhido por possuir forte integração com Inteligência Artificial e Visão Computacional.

## YOLOv8m

A escolha do modelo (Yolov8m) para detecção de objetos em tempo real, oferece alta velocidade e boa precisão na identificação de EPIs. Sendo motivada pela sua facilidade de implementação e pelo bom desempenho mesmo em computadores desktop com hardware mais simples ou menos recentes.

Além disso, versões anteriores do YOLO possuem menor custo computacional, reduzindo o tempo de treinamento e processamento das imagens. Isso permite otimizar a precisão do modelo sem comprometer significativamente o desempenho da aplicação, o armazenamento disponível e os recursos dos equipamentos utilizados no projeto.

## OpenCV

Permite captura e processamento de vídeo das câmeras industriais.

## MySQL

Banco relacional confiável para armazenamento das informações do sistema.

## React Native

Tecnologias acessíveis e eficientes para construção da interface web.

---

# Requisitos e Contexto de Uso

## Requisitos Funcionais e Não Funcionais

### Requisitos Funcionais

**RF-001: Fazer login**  
Descrição: O sistema deve exibir os campos de credenciais, como usuário e senha.  
Prioridade: Média  
Ator: Usuário  
Pré-condição: O sistema deve estar online  
Pós-condições: Usuário acessa a página inicial de dashboard

**RF-002: Acessar dashboard**  
Descrição: O sistema deve exibir os dados relacionados a segurança.  
Prioridade: Média  
Ator: Usuário  
Pré-condição: O usuário deve estar previamente logado  
Pós-condições: Usuário visualiza os dados de segurança do sistema

**RF-003: Visualizar visão**  
Descrição: O sistema deve exibir em tempo real a captura de vídeo do sistema de visão.  
Prioridade: Alta  
Ator: Usuário  
Pré-condição: O usuário deve estar previamente logado  
Pós-condições: Usuário visualiza o vídeo em tempo real

**RF-004: Alterar parâmetros da visão**  
Descrição: O usuário deve conseguir alterar os parâmetros da visão, como área de detecção e equipamentos.  
Prioridade: Média  
Ator: Usuário  
Pré-condição: O usuário deve estar previamente logado  
Pós-condições: Usuário pode alterar os parâmetros de detecção da visão

**RF-005: Notificar riscos**  
Descrição: O sistema deve notificar em caso de riscos.  
Prioridade: Média  
Ator: Usuário  
Pré-condição: O usuário deve estar previamente logado e o sistema de notificação ativo  
Pós-condições: Usuário é notificado caso haja algum risco de segurança e o sistema de notificação é ativado

**RF-006: Controlar acesso**  
Descrição: O sistema deve permitir que o administrador permita e restrinja o acesso de usuários.  
Prioridade: Média  
Ator: Administrador  
Pré-condição: O administrador deve estar previamente logado  
Pós-condições: O eventual acesso de um usuário é negado ou permitido

### Requisitos Não Funcionais

**RNF-001: Tempo de resposta da visão**  
Descrição: O sistema deve mostrar o vídeo da visão com atraso de no máximo 1 segundo.  
Prioridade: Alta  
Critério de aceitação: —

**RNF-002: Tempo de resposta das notificações**  
Descrição: O sistema deve dar prioridade a notificações e enviar a notificação em 500 ms.  
Prioridade: Alta  
Critério de aceitação: —

**RNF-003: Disponibilidade do sistema**  
Descrição: O sistema deve estar disponível em 99,9% durante o expediente.  
Prioridade: Alta  
Critério de aceitação: —

### Tabela Resumo

| ID        | Descrição                     | Tipo | Prioridade |
| ---       | ---                           | ---  | ---        |
| RF-001    | Login com credenciais         | RF   | Alta       |
| RF-002    | Visualizar dashboard          | RF   | Média      |
| RF-003    | Visualizar captura da visão   | RF   | Alta       |
| RF-004    | Alterar parâmetros da visão   | RF   | Alta       |
| RF-005    | Notificações de riscos        | RF   | Média      |
| RF-006    | Controle do acesso            | RF   | Média      |
| RNF-001   | Tempo de resposta da visão    | RNF  | Alta       |
| RNF-002   | Tempo de resposta de riscos   | RNF  | Alta       |
| RNF-003   | Disponibilidade               | RNF  | Alta       |

## Casos de Uso

## Personas

Carlos, Supervisor de Segurança do Trabalho: fica no chão de fábrica e acompanha a operação de perto. Ele acessa o sistema pelo celular ou tablet industrial e precisa receber notificações instantâneas sobre desvios de segurança, como um funcionário sem capacete. O foco dele é a intervenção imediata para proteger a equipe e prevenir acidentes.

Mariana, Gestora de Operações Industriais: atua na parte estratégica e analisa o panorama geral da fábrica. Ela acessa o dashboard pelo computador do escritório para visualizar o histórico de detecções e relatórios de conformidade. O objetivo dela é entender quais setores apresentam mais riscos e organizar campanhas de conscientização, mudando o foco da punição para a prevenção.

Roberto, Administrador do Sistema (TI): responsável pela infraestrutura e configuração técnica. Ele é a pessoa que cadastra novos funcionários, gerencia permissões e ajusta os parâmetros das câmeras, como delimitar novas áreas de risco. Ele precisa de telas de configuração claras e acesso total aos controles do sistema.

## Restrições do Sistema

Dependência de Processamento (Hardware): como a aplicação roda visão computacional pesada usando YOLOv8 e OpenCV para analisar vídeo em tempo real, o processamento não pode ser feito em máquinas comuns. O sistema exige servidores com placas de vídeo dedicadas (GPUs) ou dispositivos de computação de borda instalados na fábrica para aguentar a carga sem travar.

Condições Ambientais Físicas: a precisão da inteligência artificial depende muito da qualidade visual. Locais com pouca iluminação, excesso de poeira suspensa ou ângulos ruins onde os equipamentos bloqueiam a visão das câmeras vão diminuir a capacidade do sistema de identificar os EPIs corretamente.

Infraestrutura de Rede Local: para cumprir a meta rigorosa de entregar as notificações em 500 milissegundos e o vídeo com atraso máximo de 1 segundo, a fábrica precisa ter uma rede interna excelente. Áreas com sinal de Wi-Fi fraco ou muita interferência de maquinário pesado vão comprometer a entrega dos alertas.

---
# Conclusão 
O grupo Liora busca transformar a segurança industrial através de tecnologias inteligentes e monitoramento contínuo, promovendo prevenção de acidentes e maior eficiência operacional.
