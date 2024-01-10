# **Demonstração Prática do Data Model**

Este repositório tem como objetivo fornecer uma demonstração prática e simplificada da criação de um Data Model.

## **Descrição**

Neste projeto, foram empregadas três tabelas para a construção do Data Model. Foi feito a limpeza dos dados necessários, culminando na criação de um modelo entidade-relacionamento.

## **Guia Passo a Passo**

O guia detalhado para reproduzir o processo encontra-se no documento **DataModel.ipynb**. Siga as instruções fornecidas nesse arquivo para compreender e implementar eficientemente o Data Model proposto

---
title: accounts
---
erDiagram
accountscountry{
VARCHAR country_code PK
VARCHAR short_name
VARCHAR table_name
VARCHAR long_name
VARCHAR currency_unit
}
accountdata{
VARCHAR country_name 
VARCHAR country_code FK
VARCHAR series_name 
VARCHAR series_code FK
FLOAT YR1995 
FLOAT YR1996
FLOAT YR1997
FLOAT YR1998
FLOAT YR1999
FLOAT YR2000
FLOAT YR2001
FLOAT YR2002
FLOAT YR2003
FLOAT YR2004
FLOAT YR2005
FLOAT YR2006
FLOAT YR2007
FLOAT YR2008
FLOAT YR2009
FLOAT YR2010
FLOAT YR2011
FLOAT YR2012
FLOAT YR2013
FLOAT YR2014
FLOAT YR2015
FLOAT YR2016
FLOAT YR2017
FLOAT YR2018
}
accountseries{
VARCHAR series_code PK
VARCHAR topic
VARCHAR indicator_name
VARCHAR long_definition
}
accountscountry 1+--1+ accountdata: has
accountseries 1+--1+ accountdata: has
