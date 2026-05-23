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

![Texto Alternativo](https://github.com/VanessaRibas/Sprint1---Engenharia-de-Software/tree/main/assets/Diagrama_de_Casos_de_Uso.jpg)

## Diagrama de Atividade

![Texto Alternativo](https://github.com/VanessaRibas/Sprint1---Engenharia-de-Software/tree/main/assets/Diagrama_de_Classes.drawio.png)


## Diagrama de Classes

![Texto Alternativo](https://github.com/VanessaRibas/Sprint1---Engenharia-de-Software/tree/main/assets/Diagrama_de_Atividade.drawio.png)

---

# ⚙️ Tecnologias Selecionadas

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
# Conclusão 
O grupo Liora busca transformar a segurança industrial através de tecnologias inteligentes e monitoramento contínuo, promovendo prevenção de acidentes e maior eficiência operacional.
