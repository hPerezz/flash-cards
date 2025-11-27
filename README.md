## Flash Cards para Estudo de Provas

Este projeto é uma ferramenta simples de **flash cards** para ajudar nos estudos para provas.  
Ele carrega um banco de questões em formato **JSON** e exibe as perguntas na interface web para você praticar.

### Objetivo do Projeto

A origem deste projeto é bem prática:  
> Tenho uma prova em breve e preciso estudar.  
> Queria criar questões com IA e, para isso, pensei em pedir para as IAs criarem bancos de questões em JSON e ir somando esses bancos em `questoes.json`.
> Existem algumas ferramentas (todas pagas) que permitem criação de flashcards com IA, mas você não tem controle nenhum sobre o prompt.

Ou seja, a ideia é usar IAs (como ChatGPT, Gemini, etc.) para gerar lotes de questões e centralizar tudo em um único arquivo JSON, que a aplicação lê para montar os flash cards.

### Como adicionar ou mudar questões

Todas as questões usadas pela aplicação ficam no arquivo:

- **`questoes.json`**

Para **adicionar** ou **alterar** questões, basta editar esse arquivo:

- **Adicionar questões**:
  - Gere novas questões em formato JSON (por exemplo, usando uma IA).
  - Garanta que o formato siga a mesma estrutura dos objetos já existentes em `questoes.json`.
  - Acrescente as novas questões ao array principal do arquivo.

- **Alterar questões**:
  - Abra o `questoes.json`.
  - Localize a questão que deseja mudar.
  - Edite o enunciado, alternativas, resposta correta, explicação, ou qualquer outro campo que você esteja utilizando.

Depois de salvar o arquivo, basta recarregar a página (`flashcard.html` ou `index.html`, conforme você estiver usando) no navegador para ver as mudanças refletidas nos flash cards.

### Sugestão de uso com IA

Ao pedir para uma IA gerar questões, você pode orientar algo como:

> "Crie um banco de questões em JSON para eu estudar, seguindo o mesmo formato de objetos que já uso no meu arquivo `questoes.json`."

Depois é só copiar o array de questões retornado pela IA e mesclar dentro do `questoes.json`.  
Com o tempo, você vai construindo um grande banco de questões personalizado para revisar antes da prova.


