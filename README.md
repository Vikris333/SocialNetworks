# Social Network Graph
This project was designed to analyze social media data based on graph queries.

# 🎯 Objetivo
Este projeto tem como objetivo a criação e análise de um dataset para uma rede social utilizando o banco de dados orientado a grafos Neo4j. Consiste em simular interações entre usuários (seguidores, postagens, curtidas e comentários) para demonstrar como a estrutura de grafos facilita a extração de informações e visualização.

# 📝 Estrutura do Grafo
O dataset é composto por:
* __Nós:__ Usuário, Post, Categoria.

* __Relacionamentos:__
  * (:Usuario)-[:SEGUE]->(:Usuario)
  * (:Usuario)-[:POSTOU]->(:Post)
  * (:Usuario)-[:CURTIU]->(:Post)
  * (:Usuario)-[:COMENTOU]->(:Post)
  * (:Usuario)-[:COMPARTILHOU]->(:Post)
  * (:Post)-[:PERTENCE_A]->(:Categoria)
 
# 📊 Perguntas que este Grafo responde
Com este dataset, você pode responder a perguntas de negócio usando poucas linhas de código Cypher, como por exemplo:
* __Quem devo sugerir como amigo:__ Analisa seguidores ou interesses em comum.
* __Quantos posts um único usuário postou:__ Mostra quantos posts um usuário fez.
* __Quem são os maiores "influenciadores":__ Identifica usuários com maior número de seguidores ou maior engajamento em seus posts.
* __Quem é o público-alvo:__ Mapeia usuários que interagem com categorias específicas

   Entre muitas outras.

# 🚀 Como executar
Primeiro você precisa ter uma instância no Neo4j Desktop ou Neoj4 Aura.
   Após isso, copie e cole o script Cypher disponível neste repositório, e execute os comandos desejados (você pode encontrar e visualizar as queries para as perguntas de negócio neste repositório).
