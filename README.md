<h1>Resumo</h1><p>Sistema feito para um escritório de advocácia.</p><p><br></p><p>O intuito do sistema é cadastrar clientes, textos e blocos, para que no final um arquivo .doc seja gerado com os dados desejados.&nbsp;</p><p><br></p><p>A ideia do sistema, é um advogado ter, por exemplo, diversos textos referentes a leis.</p><p>Ele poderá criar um bloco e inserir esses textos como desejar. Esses textos podem existir em blocos diferentes.</p><p><br></p><p>Vamos supor que um texto está se referindo a uma lei que por ventura mudou, e esse texto está atrelado a vários blocos e clientes. No momento em que ele editar texto, a mudança surtirá efeito em todos os blocos de todos os clientes que contém aquele texto, facilitando a vida do advogado, onde não irá precisar mais mudar de maneira manual procurando os blocos que contém aquela determinada informação.</p><p><br></p><h1>Back-End</h1><h2>Banco de dados</h2><p>Toda a base de dados foi feita através do Prisma, usando o SQLite para armazenar os dados.</p><p>O schema é composto por três models:<strong> Client, Block, Text </strong>.</p><ul><li>Um <strong>Client </strong>pode ter vários <strong>Blocks.</strong></li><li>Um <strong>Block </strong>pode ter vários <strong>Texts.</strong></li><li><strong>Text </strong>contém uma referência não obrigatória a <strong>Blocks.</strong></li></ul><p><br></p><h2>Node.js</h2><p>Rotas criadas para o sistema:</p><ul><li><strong>Client, Block, Text </strong>- Rota <strong>get </strong>para listar um único cliente, bloco ou texto e todos os clientes, blocos ou textos.</li><li><strong>Client, Block, Text </strong>- Rota <strong>post </strong>para listar um cliente, bloco ou texto.</li><li><strong>Client, Block, Text </strong>- Rota <strong>put </strong>para editar um cliente, bloco ou texto.</li><li><strong>Client, Block, Text </strong>- Rota <strong>delete </strong>para deletar um determinado cliente, bloco ou texto(busca feita pelo id).</li><li><strong>OBS: Client, Block, Text - </strong>Para cada função citada acima, cada um possui uma rota individual.</li></ul><p><br></p><h1>Front-End</h1><h2>React</h2><p>O Next.js foi escolhido para fazer a integração do react ao sistema.</p><p>A aplicação foi feita em componentes funcionais, fazendo o uso de Hooks.</p><p>As rotas com endereços URL foram todas direcionadas através do modo no qual o Next.js trabalha.</p><p>Como mecanismo de estilização, a ferramenta TailwindCSS foi a utilizada, pela praticidade em aplicar estilos CSS.</p><p><br></p><h1>Progresso</h1><h2>Back-End</h2><p>Banco de dados: <strong>100%</strong></p><p>Rotas do server: <strong>100¨%</strong></p><p>Server: <strong>100%</strong></p><h2>Front-End</h2><p>Telas referente a Client:<strong> 100%</strong></p><ul><li>Todas as funções do CRUD</li></ul><p>Telas referente a Text:<strong> 100%</strong></p><ul><li>Todas as funções do CRUD</li></ul><p>Telas referente a Block: <strong>100%</strong></p><ul><li>Associação de Texts e Blocks</li></ul><p>Inserção da tela de Login: <strong>100%</strong></p><p>Funcionalidade de Login: <strong>0%</strong></p><p>Ferramenta parar gerar um aquivo .doc:<strong> 100%</strong></p><p><br></p>
<h1>Imagens do sistema</h1>

Versão 1.1
- Mudanças na interface foram feitas.
- A página Index foi modificada para ter utilidade, dando uma visão geral dos clientes, blocos e textos, de maneira interativa.
- Adição de variáveis genéricas, para facilitar e poupar trabalho do usuário.
- Ao criar um texto o usuário poderá utilizar essas variáveis genéricas, onde um único texto servirá para todos os clientes, onde cada cliente terá suas informações apresentadas no texto de maneira individual, como propõe o app.
- Na página de de criar texto, tem botões interativos que explicam ao usuário como funciona as variáveis genéricas.


- Nova página Index interativa.
![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/page-index-1.1.png)

- Nova tabela de clientes.
![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/client-table-1.1.png)

- Nova tabela de blocos.
![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/blocks-table-1.1.png)

- Nova tabela de textos.
![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/text-table-1.1.png)

- Variáveis genéricas contendo as informações do cliente 
![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/var-generic-1.1.png)

- Variáveis genéricas contendo as informações do cliente, em uso.
![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/var-generic-in-use-1.1.png)


Versão 1.0
![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/clients.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/texts.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/client-edit.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/client-modal.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/client-new.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/text-edit-1.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/blocks.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/block-clients.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/block-new.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/block-texts.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/block-example.png)

![alt text](https://github.com/mattmascarenhas/geradoc-1.0-complete/blob/master/img/doc-download.png)




