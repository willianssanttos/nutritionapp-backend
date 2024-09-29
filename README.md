# Documentação da API

## Introdução
Esta é uma API Node.js, que permite que os usuários gere planos de dieta comunicando-se com a API Gemini externa.

# Integração da API Gemini

## Como funciona
Envio de perfil de usuário : quando um usuário envia suas preferências alimentares por meio do /diet/generateendpoint, a API coleta esses dados e envia uma solicitação à API Gemini.

Processamento de dados : a API Gemini processa a solicitação, gera um plano de dieta personalizado com base nas preferências fornecidas e retorna o plano.

Atualizações do plano de dieta : os usuários podem atualizar suas preferências por meio da API, que regenerará o plano de dieta chamando a API Gemini novamente.

## Uso da chave API
A comunicação com a API Gemini requer uma chave de API, que deve ser armazenada no .env arquivo na raiz do projeto como API_KEY. Essa chave será usada para autenticação em cada solicitação enviada à API Gemini.