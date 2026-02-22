# 📊 Análise de Redes Sociais da Insegurança Alimentar no Brasil
# 📌 Descrição do Projeto

Este projeto aplica a metodologia de Análise de Redes Sociais (ARS) para examinar a estrutura relacional da insegurança alimentar no Brasil.

A partir da base de dados da POF 2017-2018 (52.139 observações), foi construída uma rede de coocorrência entre vulnerabilidades socioeconômicas, permitindo identificar padrões estruturais de acumulação de desvantagens.

# 🎯 Objetivo

Investigar:

* A posição estrutural das categorias de insegurança alimentar (leve, moderada e grave);

* A integração entre renda, raça, gênero e condições habitacionais;

* A existência de comunidades estruturais;

* A centralidade relativa das vulnerabilidades no sistema socioeconômico.

# 🧠 Metodologia

A análise foi realizada em R, utilizando:

* dplyr e tidyr para manipulação de dados;

* Matrix para construção da matriz de coocorrência;

* igraph para modelagem da rede;

* ggraph e ggplot2 para visualização.

# Construção da Rede

* Matriz binária indivíduo × vulnerabilidade;

* Produto matricial X'X;

* Grafo não direcionado e ponderado;

* Arestas representam número de indivíduos com duas vulnerabilidades simultâneas.

# 📈 Principais Resultados

* 13 nós e 72 arestas;

* Densidade = 0.92 (rede altamente integrada);

* Um único componente conectado;

* Modularidade = 0 (ausência de clusters bem definidos).

# Centralidade

* Variáveis de infraestrutura (LUZ_REDE, PAREDE_SOLIDA, AGUA_REDE) ocupam posições centrais;

* RENDA_BAIXA integra o núcleo estrutural;

* IS_GRAVE apresenta menor centralidade relativa;

* Ausência de nós intermediadores dominantes.

# 📊 Visualizações

O repositório inclui:

* Rede de Coocorrência da Insegurança Alimentar;

* Comunidades detectadas pelo algoritmo Louvain.

# 📌 Conclusão

Os resultados indicam que a insegurança alimentar está inserida em um sistema multidimensional altamente integrado, no qual infraestrutura domiciliar e condições materiais exercem papel estruturante central.

A Análise de Redes Sociais mostrou-se ferramenta eficaz para compreender a arquitetura relacional da vulnerabilidade socioeconômica.

📎 Referência

Caso utilize este projeto, cite como:

Meira, Maurício Almeida (2026). Análise de Redes Sociais da Insegurança Alimentar no Brasil.
