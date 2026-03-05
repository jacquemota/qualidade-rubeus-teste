# Página: Certificação
https://qualidade.apprbs.com.br/certificacao

---

BR-001 — [Formulário de inscrição] Sistema impede avanço mesmo com dados válidos

Tipo: Correção
Classificação: Utilidade
Prioridade: Alta

Descrição:
Ao preencher corretamente todos os campos obrigatórios do formulário inicial (Nome, Telefone e Email) e clicar no botão Avançar, o sistema apresenta a mensagem “é necessário informar base legal”, impedindo o usuário de prosseguir para a próxima etapa do cadastro.

A mensagem exibida não corresponde aos campos apresentados no formulário e bloqueia a continuidade do fluxo de inscrição.

Passos para reproduzir:

Acessar a página de certificação.

Preencher o campo Nome com valor válido.

Preencher o campo Telefone com número válido.

Preencher o campo Email com endereço válido.

Clicar no botão Avançar.

Resultado atual:
O sistema exibe a mensagem “é necessário informar base legal” e impede o avanço para a próxima etapa do cadastro.

Resultado esperado:
Ao preencher corretamente todos os campos obrigatórios, o sistema deve permitir o avanço para a próxima etapa do fluxo de cadastro.

Evidência:
evidencias/certificacao/BR-001.png

Página: Certificação
BR-002 — [Login/Formulário] Mensagem de erro incorreta ao informar nome inválido
Tipo: Correção
Classificação: Utilidade
Prioridade: Alta
Descrição:
Ao preencher o formulário com nome inválido e demais campos válidos, ao clicar em Avançar o sistema exibe a mensagem “é necessário informar base legal”, que não corresponde ao campo com erro. A validação atual não orienta corretamente o usuário sobre o problema no campo Nome.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Preencher o campo Nome com valor inválido.
3.	Preencher Telefone com valor válido.
4.	Preencher Email com valor válido.
5.	Clicar em Avançar.
Resultado atual:
O sistema exibe a mensagem “é necessário informar base legal” e não permite avançar.
Resultado esperado:
O sistema deve validar corretamente o campo Nome e exibir mensagem específica, por exemplo:
•	Nome completo obrigatório
•	Caracteres especiais não permitidos
•	Não aceitar formulário com apenas um nome
•	Não aceitar dois espaços entre nomes
Evidência:
evidencias/certificacao/BR-002.png

BR-003 — [Login/Formulário] Mensagem de erro incorreta ao informar número de celular inválido
Tipo: Correção
Classificação: Utilidade
Prioridade: Alta
Descrição:
Ao preencher o formulário com número de celular inválido, ao clicar em Avançar o sistema exibe a mesma mensagem genérica “é necessário informar base legal”, sem indicar que o erro está no campo Telefone.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Preencher Nome com valor válido.
3.	Preencher Telefone com número inválido.
4.	Preencher Email com valor válido.
5.	Clicar em Avançar.
Resultado atual:
O sistema exibe a mensagem “é necessário informar base legal”.
Resultado esperado:
O sistema deve identificar o erro no campo Telefone e apresentar mensagem específica, por exemplo:
•	Telefone inválido
•	Número incompleto
•	Formato de telefone inválido
Evidência:
evidencias/certificacao/BR-003.png

BR-004 — [Login/Formulário] Mensagem de erro incorreta ao informar e-mail inválido
Tipo: Correção
Classificação: Utilidade
Prioridade: Alta
Descrição:
Ao preencher o formulário com e-mail inválido, o sistema exibe a mensagem “é necessário informar base legal” após clicar em Avançar, em vez de indicar claramente a inconsistência no campo Email.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Preencher Nome com valor válido.
3.	Preencher Telefone com valor válido.
4.	Preencher Email com formato inválido.
5.	Clicar em Avançar.
Resultado atual:
O sistema exibe a mensagem “é necessário informar base legal” e não informa o erro real.
Resultado esperado:
O sistema deve validar corretamente o campo Email e exibir mensagem clara, por exemplo:
•	E-mail inválido
•	Informe um endereço de e-mail válido
Evidência:
evidencias/certificacao/BR-004.png

BR-005 — [Login/Formulário] Validação genérica impede identificação do campo com erro
Tipo: Correção
Classificação: Usabilidade
Prioridade: Alta
Descrição:
Independentemente de qual campo esteja incorreto no formulário inicial, ao clicar em Avançar o sistema exibe sempre a mesma mensagem de erro. Isso dificulta a identificação do problema e aumenta o esforço do usuário para concluir o preenchimento.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Preencher um dos campos com valor inválido.
3.	Preencher os demais campos com valores válidos.
4.	Clicar em Avançar.
Resultado atual:
O sistema exibe sempre a mesma mensagem genérica, sem indicar o campo que precisa de correção.
Resultado esperado:
O sistema deve:
•	identificar exatamente qual campo está inválido
•	destacar visualmente o campo com erro
•	exibir mensagem específica e contextualizada por campo
Evidência:
evidencias/certificacao/BR-005.png

BR-006 — [Layout] Foto com enquadramento inadequado
Tipo: Melhoria
Classificação: Desejabilidade
Prioridade: Média
Descrição:
A imagem da pessoa na área informativa da página apresenta enquadramento inadequado, com composição visual pouco equilibrada em relação ao espaço disponível. Isso reduz a qualidade estética da interface e passa sensação de acabamento inconsistente.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Observar a imagem posicionada na área esquerda da tela.
Resultado atual:
A imagem parece mal enquadrada em relação ao container e ao conteúdo textual ao redor.
Resultado esperado:
A imagem deve estar melhor centralizada e enquadrada, respeitando proporção, área visível e equilíbrio visual do bloco.
Evidência:
evidencias/certificacao/BR-006.png

BR-007 — [Layout] Alinhamento inconsistente do bloco azul do formulário
Tipo: Melhoria
Classificação: Usabilidade
Prioridade: Média
Descrição:
O bloco azul/turquesa do formulário aparenta desalinhamento em relação ao restante da composição da página, prejudicando a percepção de organização visual e consistência do layout.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Observar o posicionamento do bloco azul do formulário em relação aos textos e demais elementos da tela.
Resultado atual:
O bloco apresenta desalinhamento visual em relação ao grid da página.
Resultado esperado:
O bloco deve seguir alinhamento consistente com a estrutura visual da página, respeitando margens, respiros e proporção entre colunas.
Evidência:
evidencias/certificacao/BR-007.png

BR-010 — [UI] Border radius do bloco azul compromete a harmonia visual
Tipo: Melhoria
Classificação: Desejabilidade
Prioridade: Baixa
Descrição:
O arredondamento das bordas do bloco azul do formulário não está visualmente harmonioso com os demais elementos da interface, gerando sensação de inconsistência no design.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Observar o bloco azul do formulário e comparar o arredondamento com os demais componentes da tela.
Resultado atual:
O border radius aparenta desproporcional ou pouco refinado em relação ao restante da interface.
Resultado esperado:
O componente deve seguir um padrão visual consistente de bordas, alinhado com o design system da página.
Evidência:
evidencias/certificacao/BR-008.png

BR-009 — [UX] Ausência de mensagens de validação específicas por campo
Tipo: Melhoria
Classificação: Usabilidade
Prioridade: Média
Descrição:
O formulário não apresenta mensagens específicas próximas aos campos com erro, o que prejudica a orientação do usuário durante o preenchimento.
Passos para reproduzir:
1.	Acessar a página de certificação.
2.	Inserir valores inválidos em um ou mais campos.
3.	Clicar em Avançar.
Resultado atual:
A interface não informa claramente qual campo precisa ser corrigido nem como corrigi-lo.
Resultado esperado:
Cada campo inválido deve apresentar feedback contextual próximo ao input correspondente, com instrução objetiva de correção.
Evidência:
evidencias/certificacao/BR-009.png

BR-009 — [Certificação] Inconsistência de conteúdo entre título e seção

Tipo: Melhoria
Classificação: Usabilidade
Prioridade: Baixa

Descrição:
O botão “Quero me certificar” aparece em destaque na área superior, porém a seção abaixo não apresenta conteúdo que explique claramente o processo ou benefícios da certificação.

Isso cria uma quebra na jornada do usuário.

Passos para reproduzir:

Acessar a página inicial da certificação

Observar o botão de chamada para ação (CTA)

Resultado atual:
O botão direciona para ação sem contexto suficiente.

Resultado esperado:
A seção deve explicar:

o que é a certificação

benefícios

requisitos

etapas

Evidência:
evidencias/certificacao/BR-009.png

