# Construindo-um-esquema-conceitual-do-zero
Database Experience - Desafio 2

### Objetivo:
Cria o esquema conceitual para o contexto de oficina com base na narrativa fornecida

### Narrativa:
Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
- Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas
- Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
- A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
- O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços
- A mesma equipe avalia e executa os serviços
- Os mecânicos possuem código, nome, endereço e especialidade
- Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.

### Entidades definidas fora do escopo inicial
- TipoDocumento: Tipo do documento do cliente que será inserido, por exemplo: CPF, RG, CNPJ e ebntre outros
- Telefone: armazenar N numeros de telefone do cliente
- Especialidade: aramazenar as especialidades dos mecanicos


### Conclusão
- O cliente não foi relacionado diretamente com a Ordem de Serviço para realizar a aprovação pois o mesmo já esta relacionado com o Veiculo que esta relacionado com a Ordem de Serviço, e o campo status da Ordem de Serviço irá desmonstrar se a mesma foi ou não aprovada
- Ordem de Serviço, Peça e Servico estão relacionadas entre si repesentado o relacionamento ternário
