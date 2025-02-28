# OficinaDados

Entidades e Atributos
Cliente

Representa os clientes da oficina.

Atributos:

ID_Cliente: Identificador único do cliente.

Nome: Nome completo do cliente.

CPF: CPF do cliente (único para cada cliente).

Endereco: Endereço do cliente.

Telefone: Telefone de contato do cliente.

Veículo

Representa os veículos dos clientes que são levados para a oficina.

Atributos:

ID_Veiculo: Identificador único do veículo.

Placa: Placa do veículo (única para cada veículo).

Marca: Marca do veículo.

Modelo: Modelo do veículo.

Ano: Ano de fabricação do veículo.

ID_Cliente: Chave estrangeira que relaciona o veículo ao seu proprietário.

Ordem de Serviço (OS)

Representa as ordens de serviço geradas para cada veículo.

Atributos:

ID_OS: Identificador único da ordem de serviço.

Numero_OS: Número da ordem de serviço (único para cada OS).

Data_Emissao: Data em que a OS foi emitida.

Valor_Total: Valor total da OS (soma dos serviços e peças).

Status: Status atual da OS (Aguardando, Em andamento, Concluído).

Data_Conclusao: Data prevista para conclusão dos serviços.

ID_Veiculo: Chave estrangeira que relaciona a OS ao veículo.

ID_Equipe: Chave estrangeira que relaciona a OS à equipe responsável.

Equipe de Mecânicos

Representa as equipes de mecânicos que executam os serviços.

Atributos:

ID_Equipe: Identificador único da equipe.

Nome_Equipe: Nome da equipe.

Mecânico

Representa os mecânicos que compõem as equipes.

Atributos:

ID_Mecanico: Identificador único do mecânico.

Nome: Nome do mecânico.

Endereco: Endereço do mecânico.

Especialidade: Especialidade do mecânico (ex: motor, elétrica, suspensão).

ID_Equipe: Chave estrangeira que relaciona o mecânico à sua equipe.

Serviço

Representa os serviços que podem ser realizados na oficina.

Atributos:

ID_Servico: Identificador único do serviço.

Descricao: Descrição do serviço (ex: troca de óleo, revisão geral).

Valor_MaoDeObra: Valor da mão de obra do serviço.

Peça

Representa as peças utilizadas nos serviços.

Atributos:

ID_Peca: Identificador único da peça.

Nome: Nome da peça (ex: filtro de óleo, pastilha de freio).

Valor: Valor da peça.

Serviços da OS

Representa os serviços associados a uma ordem de serviço.

Atributos:

ID_OS: Chave estrangeira que relaciona o serviço à OS.

ID_Servico: Chave estrangeira que identifica o serviço.

Quantidade: Quantidade de vezes que o serviço será executado.

Peças da OS

Representa as peças associadas a uma ordem de serviço.

Atributos:

ID_OS: Chave estrangeira que relaciona a peça à OS.

ID_Peca: Chave estrangeira que identifica a peça.

Quantidade: Quantidade de peças utilizadas.

