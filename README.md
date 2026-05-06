# Agente de Atendimento no WhatsApp com IA + RAG

Projeto de automação criado no n8n para atendimento automático no WhatsApp utilizando IA e base de conhecimento própria.

## Tecnologias utilizadas

* n8n
* OpenAI
* Supabase Vector Store
* Google Drive
* Evolution API
* Whisper

## Como funciona

O cliente envia uma mensagem no WhatsApp

→ o sistema identifica se é texto ou áudio

→ caso seja áudio, realiza transcrição automática

→ o agente solicita o nome do cliente

→ apresenta opções de atendimento automaticamente

Exemplo:

* Produtos
* Promoções
* Trocas e devoluções
* Garantia
* Localização de lojas
* Informações da empresa

## Base de conhecimento (RAG)

Os documentos da empresa ficam armazenados no Google Drive.

Quando um novo arquivo é adicionado ou atualizado:

→ o sistema faz o download automático

→ processa o documento

→ gera embeddings

→ envia para o Supabase Vector Store

→ o agente passa a responder com base nas novas informações

## O que o agente responde

* Produtos
* Preços
* Garantias
* Trocas e devoluções
* Localização de lojas
* Informações institucionais

## Objetivo

Automatizar atendimento comercial e reduzir perda de clientes por demora nas respostas.
