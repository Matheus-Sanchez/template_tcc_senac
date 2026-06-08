---
title: "Parecer Final Consolidado da Banca"
subtitle: "Avaliação de TCC - Classificação de câncer de mama em mamografias"
author: "Banca acadêmica simulada"
date: "2026"
lang: pt-BR
geometry: margin=2.2cm
fontsize: 11pt
mainfont: DejaVu Serif
---

# Parecer final consolidado da banca

**Relator:** Professor especialista em Pesquisa Científica  
**Trabalho avaliado:** *Classificação de câncer de mama em mamografias: um estudo comparativo entre CNNs clássicas e híbridas quântico-clássicas*.

Após as nove rodadas de avaliação, a banca entende que o TCC apresenta uma proposta **relevante, atual e tecnicamente promissora**, mas ainda precisa de ajustes metodológicos e textuais importantes antes do TCC2.

O trabalho está bem posicionado ao propor uma comparação entre **CNN clássica** e **modelo híbrido quântico-clássico simulado** para classificação de mamografias. O texto demonstra consciência de que o objetivo não é criar uma ferramenta clínica de diagnóstico, mas investigar experimentalmente a viabilidade tecnológica de uma arquitetura híbrida em ambiente controlado. Essa delimitação é adequada e deve ser preservada.

## 1. Resumo geral da avaliação

A banca considera que o trabalho possui **boa maturidade conceitual para TCC1**. A introdução apresenta um problema relevante: a classificação computacional de mamografias em um contexto no qual CNNs já são amplamente usadas, mas ainda enfrentam desafios de generalização, desbalanceamento, confiabilidade e custo computacional. Ao mesmo tempo, o trabalho insere modelos híbridos quântico-clássicos como uma alternativa emergente, mas ainda exploratória, especialmente para imagens médicas de alta dimensão.

O objetivo geral é coerente com a proposta, pois declara a intenção de investigar CNNs clássicas e modelos híbridos quântico-clássicos considerando **desempenho preditivo, custo computacional, estabilidade experimental e viabilidade prática**. Os objetivos específicos também estão bem alinhados, especialmente ao prever definição da base, protocolo de pré-processamento, CNN de referência, arquitetura híbrida, número de qubits, feature map, profundidade do circuito, métricas e análise de escalabilidade.

A hipótese é um dos pontos mais bem formulados do trabalho. Ela não afirma superioridade quântica ampla; afirma que a arquitetura híbrida pode ser competitiva, limitada ou inviável dependendo das condições experimentais. Essa postura é cientificamente adequada, porque permite que resultados negativos também sejam interpretados como contribuição válida.

A proposta metodológica é boa, principalmente por incluir três arquiteturas: **CNN clássica**, **CNN com gargalo clássico equivalente** e **modelo híbrido quântico-clássico**. A banca considerou a CNN com gargalo clássico um ponto metodológico muito forte, pois permite avaliar se eventual diferença de desempenho vem do componente quântico ou apenas da redução dimensional necessária para alimentar o circuito.

## 2. Principais pontos fortes

### 2.1 Relevância social e acadêmica

O tema é socialmente relevante por estar relacionado ao câncer de mama e à mamografia, área em que a detecção precoce possui impacto importante. O texto reconhece que a interpretação de mamografias é complexa, envolvendo massas, microcalcificações, assimetrias, distorções arquiteturais, densidade mamária, qualidade da aquisição e variação entre pacientes.

Do ponto de vista acadêmico, o trabalho é relevante porque combina **visão computacional médica**, **aprendizado profundo** e **aprendizado de máquina quântico**, sem tratar a computação quântica como solução mágica. A revisão mostra cautela ao reconhecer que modelos híbridos ainda carecem de validação comparativa rigorosa em aplicações médicas.

### 2.2 Hipótese cientificamente prudente

A banca valorizou a forma como a hipótese foi construída. O texto afirma que não se pressupõe superioridade geral da abordagem quântica e que o objetivo é investigar em quais condições ela pode ser competitiva, limitada ou inviável.

Essa formulação protege o trabalho de uma crítica comum em pesquisas com tecnologias emergentes: prometer vantagem antes de demonstrar evidência.

### 2.3 Boa estrutura de revisão teórica

A revisão bibliográfica cobre os principais blocos necessários: câncer de mama, mamografia, bases de dados, imagens digitais, classificação supervisionada, métricas, CNNs, aumento de dados, Grad-CAM, computação quântica, modelos variacionais, limitações NISQ e trabalhos correlatos. O sumário mostra uma progressão lógica do domínio médico para o domínio computacional e, depois, para o domínio quântico.

A metodologia da pesquisa bibliográfica também é positiva, pois menciona bases de busca, palavras-chave em português e inglês, operadores booleanos, blocos temáticos e critérios de inclusão. Além disso, prevê uma matriz de revisão com ano, autores, base, método, tarefa, métricas, contribuições e relação com o TCC.

### 2.4 Controle experimental com gargalo clássico

Este foi considerado o ponto metodológico mais forte do trabalho. A proposta de comparar o modelo híbrido não apenas com uma CNN completa, mas também com uma CNN com gargalo clássico equivalente, torna o experimento mais justo.

Esse controle evita uma conclusão equivocada, como atribuir ao circuito quântico um efeito que poderia ser causado apenas pela compactação das características.

### 2.5 Critérios de validação adequados

A banca considerou adequada a escolha de **AUC macro, F1-score macro e recall da classe maligna** como métricas principais, tratando acurácia como métrica complementar. Essa decisão é coerente com o problema, pois a acurácia pode ser enganosa em bases desbalanceadas. O uso da matriz de confusão para analisar falsos negativos da classe maligna também é pertinente.

### 2.6 Consciência das limitações quânticas

O texto demonstra boa cautela ao discutir codificação de dados, número reduzido de qubits, custo de simulação, profundidade de circuito, shots, ruído e barren plateaus. Também reconhece que a codificação direta de uma mamografia de alta resolução é impraticável, exigindo extração de características ou redução dimensional.

## 3. Principais pontos fracos

### 3.1 O resumo precisa ser reescrito

O resumo atual ainda tem linguagem informal e pouco acadêmica. Expressões como “chute aleatório”, “classificar mais exames radiográficos” e “precisão de cerca de 70 por cento na média” precisam ser substituídas por formulações técnicas.

Além disso, “precisão” pode gerar ambiguidade: em aprendizado de máquina, precisão não é o mesmo que acurácia. O resumo precisa declarar exatamente qual métrica foi obtida no trabalho anterior.

### 3.2 Falta uma pergunta de pesquisa explícita

Embora o texto diga que apresenta a pergunta de pesquisa, a banca recomenda que ela apareça de forma destacada, em uma frase direta. A ausência de uma pergunta bem visível reduz a força metodológica da introdução.

Formulação sugerida:

> Em uma tarefa controlada de classificação multiclasse de mamografias, uma arquitetura híbrida quântico-clássica simulada apresenta desempenho, estabilidade e custo computacional competitivos em relação a uma CNN clássica?

### 3.3 “Competitivo” ainda está vago

O texto afirma que o modelo híbrido será considerado competitivo se apresentar desempenho próximo ao baseline clássico, especialmente em AUC macro, F1 macro e recall da classe maligna, sem aumento desproporcional de custo computacional.

O problema é que “próximo” e “desproporcional” ainda não têm definição objetiva. A banca recomenda estabelecer margens numéricas antes dos experimentos.

### 3.4 A arquitetura quântica ainda precisa ser especificada

A proposta fala em circuito quântico variacional simulado, mas ainda não define suficientemente:

| Elemento | Deve ser especificado |
|---|---|
| Número de qubits | 2, 4, 6, 8 etc. |
| Codificação | RY encoding, ZZFeatureMap, PauliFeatureMap etc. |
| Ansatz | RealAmplitudes, EfficientSU2, TwoLocal etc. |
| Profundidade | número de repetições |
| Backend | Statevector, AerSimulator, Sampler, Estimator |
| Shots | simulação ideal ou com amostragem |
| Otimizador | Adam, COBYLA, SPSA etc. |
| Saída | valores esperados, probabilidades ou bitstrings |

Sem isso, a parte Qiskit ainda fica conceitual demais.

### 3.5 Divisão dos dados precisa ser mais rigorosa

O texto menciona que, “sempre que possível”, a divisão buscará evitar vazamento entre treino, validação e teste quando houver metadados de paciente ou exame.

A banca considera essa expressão fraca. Se houver metadados de paciente ou exame, a divisão deve obrigatoriamente evitar vazamento. Caso não seja possível, isso precisa ser declarado como ameaça à validade.

### 3.6 Falta uma seção de ameaças à validade

O trabalho precisa reconhecer formalmente riscos metodológicos, como:

- vazamento de dados;
- desbalanceamento de classes;
- ausência de validação externa;
- poucas execuções por modelo;
- dependência de simulação ideal;
- limitação de hardware;
- dificuldade de generalizar resultados para uso clínico.

### 3.7 Falta formalização matemática mais explícita

A banca de matemática recomenda inserir uma subseção de formulação matemática do problema, incluindo:

- definição da tarefa como classificação supervisionada;
- função do modelo;
- saída softmax;
- função de perda;
- regra de decisão;
- métricas principais.

Isso fortalecerá a defesa diante de perguntas sobre precisão, recall, F1, AUC, entropia cruzada e critérios de comparação.

## 4. Mudanças recomendadas

A banca recomenda as seguintes mudanças no texto:

1. **Reescrever o resumo em linguagem acadêmica**, retirando expressões informais e definindo corretamente métricas.

2. **Inserir uma pergunta de pesquisa explícita** no final da introdução.

3. **Adicionar uma seção “Contribuições esperadas do trabalho”**, com 3 ou 4 contribuições objetivas:
   - construção de pipeline experimental comparativo;
   - implementação de CNN clássica, CNN com gargalo e modelo híbrido;
   - análise de desempenho, custo, estabilidade e escalabilidade;
   - avaliação crítica da viabilidade de QML em mamografias.

4. **Criar uma subseção “Caracterização da pesquisa”**, classificando o estudo como:
   - pesquisa aplicada;
   - abordagem quantitativa;
   - objetivo exploratório e experimental;
   - procedimento experimental comparativo com implementação computacional.

5. **Definir critérios objetivos de competitividade**, por exemplo:
   - diferença máxima aceitável de F1 macro;
   - diferença máxima aceitável de AUC macro;
   - margem aceitável para recall da classe maligna;
   - limite aceitável de custo computacional.

6. **Especificar a arquitetura da CNN clássica**, incluindo camadas, filtros, funções de ativação, pooling, dropout, batch normalization, otimizador, taxa de aprendizado, batch size e número de épocas.

7. **Especificar o componente quântico em Qiskit**, incluindo feature map, ansatz, backend, shots, número de qubits e estratégia de treinamento.

8. **Transformar o baseline com gargalo clássico em elemento central da metodologia**, pois ele é uma das maiores forças do trabalho.

9. **Formalizar matematicamente a tarefa de classificação**, a função de perda e as métricas.

10. **Adicionar uma seção “Ameaças à validade”**, separando validade interna, externa, de construto e de conclusão.

11. **Criar um plano de contingência técnica**, principalmente para riscos envolvendo Qiskit, tempo de simulação, memória e convergência do circuito.

12. **Fixar uma política de reprodutibilidade**, com seeds, salvamento dos splits, versões das bibliotecas, logs de treino e arquivos de configuração.

## 5. Ajustes prioritários antes do TCC2

A banca recomenda priorizar os ajustes nesta ordem:

| Prioridade | Ajuste | Justificativa |
|---:|---|---|
| 1 | Reescrever o resumo | É a primeira parte lida pela banca e hoje está abaixo do nível do restante do texto |
| 2 | Formular pergunta de pesquisa explícita | Dá unidade lógica ao trabalho |
| 3 | Definir critério objetivo de “competitivo” | Evita conclusão subjetiva |
| 4 | Especificar arquitetura CNN e arquitetura híbrida | Torna a metodologia implementável |
| 5 | Definir protocolo de divisão dos dados | Reduz risco de vazamento e crítica metodológica grave |
| 6 | Criar seção de ameaças à validade | Mostra maturidade científica |
| 7 | Detalhar Qiskit: feature map, ansatz, backend e shots | Fortalece a parte quântica |
| 8 | Formalizar métricas e função de perda | Melhora rigor matemático |
| 9 | Criar plano de contingência | Protege o TCC caso o modelo híbrido não convirja |
| 10 | Organizar matriz dos trabalhos relacionados | Fortalece a lacuna científica |

## 6. Parecer final sobre a continuidade do projeto

A banca emite parecer **favorável à continuidade do projeto**, com ressalvas metodológicas.

O trabalho possui tema relevante, boa fundamentação inicial, hipótese prudente e proposta metodológica promissora. A comparação entre CNN clássica, CNN com gargalo clássico e modelo híbrido quântico-clássico simulado é defensável e adequada para um TCC de Ciência da Computação. A inclusão de custo computacional, estabilidade e escalabilidade torna o estudo mais forte do que uma simples comparação por acurácia.

Contudo, para o TCC2, o aluno precisa transformar a proposta em um protocolo experimental mais objetivo, auditável e reprodutível. O risco principal não está no tema, mas na execução: se arquitetura, métricas, splits, critérios de competitividade e configurações quânticas não forem definidos antes dos experimentos, a conclusão poderá ficar frágil.

**Parecer consolidado:** o projeto deve prosseguir para o TCC2, desde que sejam realizados os ajustes indicados, especialmente na metodologia experimental, na especificação do componente quântico e na definição objetiva dos critérios de comparação. A banca entende que mesmo um resultado em que o modelo híbrido seja inferior à CNN clássica poderá constituir contribuição válida, desde que a análise seja bem controlada, crítica e metodologicamente transparente.
