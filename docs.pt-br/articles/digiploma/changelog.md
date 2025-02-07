﻿# Histórico de versões do Digiploma

> [!NOTE]
> Este histórico por ora contém informações apenas sobre as atualizações mais recentes ao sistema. Estamos
> trabalhando para documentar as versões mais antigas.

<a name="v2-8-1" />
### 2.8.1 (2023-02-27)

* Correções de bugs
  * [AUT-303] JSON de emissão sem documentação comprobatória não é validado corretamente

* Melhorias
  * [AUT-301] Tornar opcional o campo ProcessoDoDiploma em LivroRegistro
  * [AUT-302] Informações do ato regulatório não está aparecendo no RVHE

* Novas funcionalidades
  * [AUT-299] Criar tag de Ênfase no RVDD

<a name="v2-8-0" />
### 2.8.0 (2023-02-14)

* Correções de bugs
  * [AUT-298] Corrigir erros identificados na versão 1.05 em homologação

* Novas funcionalidades
  * [AUT-270] Atualizar Diploma Digital para a versão 1.05
  * [AUT-271] Atualizar Documentação Acadêmica para a versão 1.05
  * [AUT-272] Atualizar Histórico Escolar para a versão 1.05

<a name="v2-7-0" />
### 2.7.0 (2023-01-19)

* Correções de bugs
  * [AUT-293] Erro ao gerar RVHE para Disciplina com Aprovação nula
  * [AUT-295] Data de publicação no RVHE incorreta

* Melhorias
  * [AUT-294] Adicionar validação se data de expedição está na vigência da versão atual
  * [AUT-297] Atualizar framework para .NET 6

* Novas funcionalidades
  * [AUT-291] Implementar a anulação temporária para histórico escolar

<a name="v2-6-0" />
### 2.6.0 (2022-12-21)

* Correções de bugs
  * [AUT-290] Erro ao gerar histórico escolar de emissão anterior a melhoria de informações faltantes

* Melhorias
  * [AUT-284] Relatório de documentos no SysAdmin
  * [AUT-285] Emissões de histórico no relatório
  * [AUT-288] Adicionar coluna Forma de Integralização da disciplina no RVHE
  * [AUT-289] Refatorar a validação do elemento Assinantes

<a name="v2-5-0" />
### 2.5.0 (2022-12-12)

* Correções de bugs
  * [AUT-279] Erro quando não é informado ato regulatório para instituição que não pertence ao sistema federal
  * [AUT-281] Elemento de informações adicionais é adicionado com valor vazio utilizando CSV

* Melhorias
  * [AUT-227] Melhorar validação do código de verificação no momento de registro
  * [AUT-275] Reconhecimento dos dados do Curso não deve ser obrigatório para histórico escolar
  * [AUT-278] Remover obrigatoriedade da nota das disciplinas
  * [AUT-280] Incluir a data de publicação do D.O.U nas informações de reconhecimento de curso no RVHE
  * [AUT-282] Criar checkbox para desabilitar validação das assinaturas

* Novas funcionalidades
  * [AUT-264] Criar status "Aguardando aceitação" para organização Registradora
  * [AUT-286] Criar tag para informar apenas a data da habilitação no RVDD

<a name="v2-4-1" />
### 2.4.1 (2022-11-16)

* Correções de bugs
  * [AUT-207] Adicionar DataRegistro e Descricao de Atividade complementar no CSV
  * [AUT-263] Arquivos da documentação comprobatória não são salvos para Doc. Acadêmica NSF
  * [AUT-265] Erro na validação do campo Assinantes
  * [AUT-268] Alterar o tipo da resposta da API de cancelamento da Lyceum

* Melhorias
  * [AUT-261] Criar API para listar histórico escolares de um lote

<a name="v2-4-0" />
### 2.4.0 (2022-11-08)

* Correções de bugs
  * [AUT-231] Não é possível utilizar a opção "Nova Pasta" ao registrar diplomas
  * [AUT-247] Tipo da situação atual do discente não é preenchida no XML do Histórico
  * [AUT-250] O texto de rodapé do RVHE está por cima das informações dos elementos históricos
  * [AUT-255] Hora de emissão no RVHE está em GMT
  * [AUT-256] Registro não é concluído caso já exista Histórico Escolar do mesmo aluno na IES Emissora
  * [AUT-258] Não é retornado Nonce em Doc. Academica NSF

* Melhorias
  * [AUT-226] Adicionar geração de histórico escolar no gerador
  * [AUT-237] Gerar XMLs codificados em UTF-8
  * [AUT-240] Adicionar nos testes possibilidade de gerar lista de tags do RVDD
  * [AUT-241] Implementar nos testes possibilidade de gerar RVDD de Documentação Acadêmica
  * [AUT-243] Adicionar informações faltantes ao RVHE
  * [AUT-248] Remover coluna Pendente da representação visual do Histórico Escolar
  * [AUT-249] Página de detalhes do modelo encaminhando para página errada ao clicar em "Gerar Diplomas"
  * [AUT-257] Retirar texto "Ministerial" para Portaria nos atos regulatórios
  * [AUT-260] Melhorar a lista de modelos na criação de diplomas ou históricos
  * [AUT-262] Alterar endpoint de cancelamento da Lyceum

* Novas funcionalidades
  * [AUT-252] Criar API para gerar RVHE novamente
  * [AUT-253] Erro ao gerar histórico escolar com diploma utilizando lote de diplomas por CSV

<a name="v2-3-1" />
### 2.3.1 (2022-10-06)

* Correções de bugs
  * [AUT-236] Tela de revisão não carrega quando a situação é não habilitado no Enade
  * [AUT-234] Não é possível gerar RVHE caso exista Estágio sem concedente

* Melhorias
  * [AUT-101] Tratar o caso do diploma ter sido excluido no signer ao anular diploma

* Novas funcionalidades
  * [AUT-239] Criar tag que retorne de forma dinâmica o documento de identificação juntamente com o tipo
  * [AUT-238] Criar tag para retornar texto tipo de ato regulatório em tramitação

Atualiza modelo do banco de dados: não

<a name="v2-3-0" />
### 2.3.0 (2022-10-01)

* Correções de bugs
  * [AUT-210] Conversão para dados mínimos da mantenedora não verifica se valor é nulo

* Melhorias
  * [AUT-233] Verificar se emissão possui informações sobre histórico escolar
  * [AUT-228] Permitir apenas que diplomas de 1º via gerem histórico automaticamente
  * [AUT-222] Unificar código que lança erro referente ao tipo esperado de template
  * [AUT-221] Adicionar validações referentes ao template do histórico
  * [AUT-218] Adicionar rota do histórico como filha da rota de detalhes do diploma

* Novas funcionalidades
  * [AUT-230] Gerar XMLs sem espaços e quebras de linha
  * [AUT-229] Criar API para criar histórico de forma unitária
  * [AUT-225] Validar o fluxo enviado quando criar um diploma pela API
  * [AUT-220] Adicionar documentação do histórico e novos webhooks ao Swagger
  * [AUT-217] Criar constante com mensagem de cancelamento automático para registro
  * [AUT-200] Permitir que diplomas de Emissoras com Lyceum sejam registrados por Integração
  * [AUT-195] Implementar o XML de Histórico Escolar

Atualiza modelo do banco de dados: sim

<a name="v2-2-6" />
### 2.2.6 (2022-09-20)

* Novas funcionalidades
  * [AUT-214] Criar API para reenviar webhooks

Atualiza modelo do banco de dados: não

<a name="v2-2-5" />
### 2.2.5 (2022-09-15)

* Correções de bugs
  * [AUT-213] A aplicação está permitindo a criação de diploma com HoraAula com valor 0
  * [AUT-212] Não é apresentado erro quando é enviado Enade sem Edição
  * [AUT-211] Tela de revisão não carrega caso possua estágio sem concedente

* Melhorias
  * [AUT-209] Remover referência a template ao anular Emissão
  * [AUT-198] Validar se XML da documentação acadêmica está assinado

Atualiza modelo do banco de dados: não

<a name="v2-2-4" />
### 2.2.4 (2022-09-12)

* Correções de bugs
  * [AUT-208] Remover obrigatoriedade da documentação comprobatória em diplomas de segunda via

Atualiza modelo do banco de dados: não

<a name="v2-2-3" />
### 2.2.3 (2022-09-06)

* Melhorias
  * [AUT-197] Melhorar a usabilidade no preenchimento das informações da IES Registradora

Atualiza modelo do banco de dados: não

<a name="v2-2-2" />
### 2.2.2 (2022-08-30)

* Correções de bugs
  * [AUT-206] Tela de revisão não carrega quando não existe Termo de Responsabilidade

Atualiza modelo do banco de dados: não

<a name="v2-2-1" />
### 2.2.1 (2022-08-30)

* Correções de bugs
  * [AUT-204] Data de publicação duplicada

Atualiza modelo do banco de dados: não

<a name="v2-2-0" />
### 2.2.0 (2022-08-25)

* Correções de bugs
  * [AUT-201] Mensagem de erro ao enviar "Psicólogo" em OutroTitulo

* Novas funcionalidades
  * [AUT-189] Relatório de diplomas por período

Atualiza modelo do banco de dados: não

<a name="v2-1-2" />
### 2.1.2 (2022-08-10)

* Correções de bugs
  * [AUT-181] Datas 01/01/0001 estão sendo permitidas pelo sistema

* Melhorias
  * [AUT-184] Não permitir assinatura de diplomas sem assinatura de e-CPF
  * [AUT-177] Melhorar a validação de textos que iniciam com espaço

* Novas funcionalidades
  * [AUT-76] Personalizar página de validação por organização

Atualiza modelo do banco de dados: não

<a name="v2-1-1" />
### 2.1.1 (2022-04-28)

* Correções de bugs
  * [AUT-178] Erro na escrita por extenso de alguns estados

* Melhorias
  * [AUT-180] Atualizar a condicional do texto de Naturalidade
  * [AUT-167] Melhorar a leitura de JSON com campos vazios

Atualiza modelo do banco de dados: não

<a name="v2-0-0" />
### 2.0.0 (2022-04-04)

* Correções de bugs
  * [AUT-150] Botão de envio desabilitado ao tentar enviar documentação

* Melhorias
  * [AUT-173] Criação de tag para data de colação por extenso
  * [AUT-164] Especificar CultureInfo em conversões de data para string
  * [AUT-162] Atualizar os campos informados na tela de validação
  * [AUT-152] Adicionar coluna de IES Emissora na tela da registradora
  * [AUT-151] Botão "Ir para assinador" somente para Administrador e Gerente
  * [AUT-149] Melhorar opção de deletar documento carregado
  * [AUT-146] "Não gerar" na lista de RVDD como última opção
  * [AUT-145] Esclarecer texto do campo para definir assinatura de PJ no fluxo

* Novas funcionalidades
  * [AUT-147] Pré-visualização dos documentos enviados
  * [AUT-134] Criação de Parcerias na administração de subscription
  * [AUT-133] Diferenciar lote por tipo
  * [AUT-132] Revisão de registro
  * [AUT-130] Listagem de Registros
  * [AUT-129] Permitir configurar dados da registradora
  * [AUT-128] Configurações de Integração de Emissora e Registradora
  * [AUT-127] Tela de listagem e criação de Emissões
  * [AUT-126] Permitir separar organizações por tipo
  * [AUT-125] Permitir separar tipos de fluxo por tipo

Atualiza modelo do banco de dados: sim

<a name="v1-14-0" />
### 1.14.0 (2022-04-07)

* Correções de bugs
  * [AUT-166] Seção não é retornada quando a Pagina não possui informação

* Melhorias
  * [AUT-171] Criar tag para texto relacionado ao processo de tramitação

* Novas funcionalidades
  * [AUT-176] Permitir atualização de RVDD de vários diplomas
  * [AUT-163] Tag de Segunda Via no RVDD

Atualiza modelo do banco de dados: não

<a name="v1-13-1" />
### 1.13.1 (2022-02-23)

* Melhorias
  * [AUT-161] Caractere pipe como quebra de linha na tag de Informação Adicional

Atualiza modelo do banco de dados: não

<a name="v1-13-0" />
### 1.13.0 (2022-02-14)

* Correções de bugs
  * [AUT-156] Obrigatoriedade indevida de campos na emissão de 2ª via
  * [AUT-154] Habilitação não é retornada no RVDD ao enviar mais de um nome

* Melhorias
  * [AUT-155] Permitir o uso de outras tags no Caminho de Validação

Atualiza modelo do banco de dados: não

<a name="v1-12-0" />
### 1.12.0 (2022-01-26)

* Correções de bugs
  * [AUT-143] Versão do diploma errada ao enviar webhook
  * [AUT-142] Erro de validação em regex do numero do ato

* Melhorias
  * [AUT-141] Permitir ter URLs com caminhos na URL base do modelo
  * [AUT-140] Criar novas chaves para o RVDD
  * [AUT-139] Melhorar mensagem de erro ao não preencher um campo uint como número processo da informacoesTramitacaoEmec

Atualiza modelo do banco de dados: não

<a name="v1-11-1" />
### 1.11.1 (2022-01-18)

* Correções de bugs
  * [AUT-138] Erro ao recuperar informações da documentação de registro

* Melhorias
  * [AUT-137] Novas chaves para data no RVDD e nova coluna na Pré-Visualização do aluno

Atualiza modelo do banco de dados: não

<a name="v1-11-0" />
### 1.11.0 (2021-11-30)

* Melhorias
  * [AUT-120] Adequações para versão 1.03 do XSD
  * [AUT-121] CPF do diplomado mascarado na tela de validação

Atualiza modelo do banco de dados: não

> [!WARNING]
> Breaking changes da API:
> TituloConferido: o valor "Psicólogo" não pode ser utilizado na propriedade "outroTitulo", já que foi adicionado à enum Titulo.
> DisciplinaCursada: adicionada nova propriedade obrigatória "situacao" (SituacaoDisciplina).
> "tipoAvaliacao" passa ser opcional e teve os valores "Aprovado" e "Reprovado" movidos para propriedade "situacao". Foram adicionados os valores "ConceitoRM" e "ConceitoEspecificoDoCurso".

<a name="v1-10-0" />
### 1.10.0 (2021-11-11)

* Melhorias
  * [AUT-114] Anulação definitiva de diplomas

Atualiza modelo do banco de dados: não

<a name="v1-9-2" />
### 1.9.2 (2021-11-05)

* Correções de bugs
  * [AUT-118] Chave NacionalidadeGenero faz flexão de gênero apenas se a nacionalidade informada no diploma estiver no masculino
  * [AUT-117] Mensagens de erro de RG, Outro documento de identificação, naturalidade e Situação ENADE não exibem o caminho correto
  * [AUT-116] Termo responsabilidade não deveria ser obrigatório
  * [AUT-115] Erro ao gerar diploma sem livro registro
  * [AUT-113] Correções das chaves para geração de RVDD

Atualiza modelo do banco de dados: não

<a name="v1-9-1" />
### 1.9.1 (2021-10-21)

* Correções de bugs
  * [AUT-112] Recredenciamento está como obrigatório na IES Emissora

Atualiza modelo do banco de dados: não

<a name="v1-9-0" />
### 1.9.0 (2021-10-20)

* Novas funcionalidades
  * [AUT-111] Novos condicionais e flexões de gênero

* Correções de bugs
  * [AUT-110] Erro ao enviar diploma com enums sem acento
  * [AUT-109] Erro ao gerar diploma sem Autorizacao, Reconhecimento e Renovação
  * [AUT-108] Dados do reconhecimento estão sendo exibidos como sendo da renovação de reconhecimento

Atualiza modelo do banco de dados: não

<a name="v1-8-0" />
### 1.8.0 (2021-10-13)

* Novas funcionalidades
  * [AUT-106] Adicionar upload de novo arquivo no modelo para impressão em papel timbrado

Atualiza modelo do banco de dados: sim

<a name="v1-7-0" />
### 1.7.0 (2021-10-01)

* Novas funcionalidades
  * [AUT-103] Adicionar filtro por status e data na listagem de diplomas

* Melhorias
  * [AUT-104] Adicionar nova chave para fazer flexão de gênero do titulo conferido ao estudante
  * [AUT-100] Aceitar flow id na API de criação de diplomas

* Correções de bugs
  * [AUT-105] Tela de validação apresenta erros caso o diploma não esteja válido

Atualiza modelo do banco de dados: não

<a name="v1-6-0" />
### 1.6.0 (2021-09-17)

* Novas funcionalidades
  * [AUT-95] Download em lote dos documentos de Diploma
  * [AUT-26] Captcha de proteção para consulta pública

* Melhorias
  * [AUT-93] Assinatura de diploma com requisitos de certificados

Atualiza modelo do banco de dados: não
