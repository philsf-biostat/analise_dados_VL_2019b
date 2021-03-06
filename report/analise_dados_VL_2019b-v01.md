---
title: "Análise Estatística de ..."
author: '**De:** Felipe Figueiredo **Para:** Victor Lima'
date: '**Data: ** dd/mm/aaaa'
output:
  html_document:
    fig_caption: yes
    fig_height: 6
    fig_width: 6
    keep_md: yes
    number_sections: yes
    toc: yes
  pdf_document:
    number_sections: yes
    toc: yes
  word_document:
    fig_caption: yes
    fig_height: 6
    fig_width: 6
    reference_docx: misc/style.docx
    toc: yes
subtitle: 'RELATÓRIO: analise_dados_VL_2019-v01a'
toc-title: "Sumário"
---



---

**Histórico do documento**


Versão   Alterações     
-------  ---------------
01       Versão inicial 

---

# Assinaturas


Papel             Nome   Função   Assinatura                   Data          
----------------  -----  -------  ---------------------------  --------------
Elaborador        Nome   Função   __________________________   _____________ 
Revisado por                      __________________________   _____________ 
Aprovação final                   __________________________   _____________ 



# Lista de abreviaturas

# Introdução

## Objetivos

## Recepção e tratamento dos dados

# Metodologia

## Tamanho do estudo

O cálculo do tamanho da amostra de um estudo requer a estipulação prévia do tamanho do efeito que os pesquisadores presumem ser possível detectar.
Na ausência de estudos descritivos prévios estabelecendo as estatísticas descritivas típicas para determinação de tamanhos de efeito absolutos no cenário específico de um estudo, a determinação de um tamanho de efeito absoluto pode ser um desafio, pois nem sempre a média ou a variabilidade da população são conhecidas antes da intervenção do estudo.
Na abordagem de Cohen (1988) de tamanhos de efeitos relativos utiliza-se a diferença normalizada **d** que é relativa à variabilidade na população alvo.
Esta abordagem permite calcular tamanhos de amostra para detectar efeitos considerados pequenos (d em torno de 0.2 ou 0.3), médios (d em torno de 0.5) ou grandes (d em torno de 0.8 ou 1).
Mas mesmo presumindo que TXA tenha tenha efeito relativo médio (em torno de d=0.5) no volume drenado pós-operatório, precisamos ainda diferenciar as particularidades da ritidoplastia e da mastoplastia.
Como a área acometida na mastoplastia é substancialmente maior que na ritidoplastia, é razoável que haja mais variabilidade observável no volume drenado naquele procedimento o que pode dificultar a detecção do efeito do TXA, quando comparado à ritidoplastia.
Estipulamos assim um efeito relativo para mastoplastia (d=0.4) ligeiramente menor do que para ritidoplastia (d=0.6).
Para atingir poder de 80% ao nível de 5% de significância em um estudo pareado são necessários aproximadamente N=50 participantes de mastoplastia (d=0.4) e aproximadamente N=23 participantes de ritidoplastia (d=0.6).
Assim o tamanho total do estudo é de N=73 participantes.

## Variáveis coletadas

## Análise estatística

Esta análise foi realizada utilizando-se o software `R` versão 3.6.2.

# Resultados

## Descrição da amostra de estudo


-----------------------------
      Group          value   
----------------- -----------
  Observations               

                      38     

      SEXO                   

        F          100% (38) 

        M           0% (0)   

     missing        0% (0)   

      IDADE                  

       yes          0% (0)   

       no           0% (0)   

     missing       100% (38) 

     ALTURA                  

       yes          0% (0)   

       no           0% (0)   

     missing       100% (38) 

      PESO                   

       yes          0% (0)   

       no           0% (0)   

     missing       100% (38) 

       IMC                   

    Mean (SD)      NaN (NA)  

 valid (missing)    0 (38)   
-----------------------------

Table: **Tabela 1** Características demográficas da amostra do estudo piloto.

## Efetividade do tratamento


------------------------------------------------------------------------------
        &nbsp;                ctr             txa          p     test    SMD  
----------------------- --------------- --------------- ------- ------ -------
         **n**                38              38                              

 **dreno (mean (SD))**   52.71 (18.63)   46.58 (15.90)   0.127          0.354 
------------------------------------------------------------------------------

Table: **Tabela 2** Avaliação da efetividade do tratamento com áxido tranexâmico (txa) em comparação ao lado controle (ctr);
SMD = standardized mean difference -- estimativa do tamanho do efeito observado

<!-- # Exceções e Desvios do teste -->

# Conclusões


# Referências

# Apêndice

