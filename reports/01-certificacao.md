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


BR-011 — [Rodapé / Outros Cursos] Inconsistência no texto do botão do card

Tipo: Correção
Classificação: Usabilidade
Prioridade: Média

Descrição:
O primeiro card apresenta o botão "Saiba", enquanto os outros cards utilizam "Saiba mais". Isso cria inconsistência de interface e quebra o padrão visual da seção.

Interfaces consistentes facilitam a leitura e reduzem a carga cognitiva do usuário.

Passos para reproduzir

Acessar a seção Outros Cursos

Observar os três cards apresentados

Resultado atual

Card 1 → "Saiba"

Card 2 → "Saiba mais"

Card 3 → "Saiba mais"

Resultado esperado

Todos os cards devem utilizar o mesmo padrão de texto, preferencialmente:

"Saiba mais"

BR-013 — [Outros Cursos] Alinhamento inconsistente entre imagem e conteúdo do card

Tipo: Melhoria
Classificação: Usabilidade
Prioridade: Baixa

Descrição

A área de imagem e a área inferior do card possuem cortes visuais diferentes, criando a sensação de desalinhamento entre as seções do componente.

Isso pode ser causado por:

diferença de padding

diferença de altura das imagens

overlay mal aplicado

Passos para reproduzir

Acessar a seção Outros Cursos

Comparar visualmente os três cards

Resultado atual

Os cards apresentam leve inconsistência entre:

altura das imagens

alinhamento da área inferior azul

Resultado esperado

Todos os cards devem possuir:

mesma altura de imagem

alinhamento uniforme entre imagem e área inferior

BR-012 — [Outros Cursos] Sombreamento inconsistente entre os cards

Tipo: Melhoria
Classificação: Desejabilidade
Prioridade: Baixa

Descrição

Os cards possuem sombra aplicada, porém a intensidade do sombreamento cria um leve efeito de profundidade irregular na interface.

Isso pode gerar sensação de desalinhamento ou inconsistência entre os componentes.

Passos para reproduzir

Acessar a seção Outros Cursos

Comparar visualmente as sombras dos três cards

Resultado atual

As sombras apresentam percepção visual levemente irregular.

Resultado esperado

Utilizar um único padrão de sombra para todos os cards, garantindo consistência visual.

BR-015 — [Outros Cursos] Overlay escuro da imagem reduz contraste do conteúdo

Tipo: Melhoria
Classificação: Usabilidade
Prioridade: Baixa

Descrição

As imagens dos cursos possuem um overlay escuro aplicado, porém em alguns casos o contraste pode prejudicar a visibilidade do texto.

Isso ocorre porque:

cada imagem possui luminosidade diferente

o overlay possui opacidade fixa

Passos para reproduzir

Acessar a seção Outros Cursos

Observar contraste entre texto e imagem

Resultado atual

Alguns cards apresentam contraste menor entre texto e imagem.

Resultado esperado

Aplicar um overlay com opacidade ajustada ou um gradiente mais consistente para garantir legibilidade.

BR-014 — [Rodapé] Desbalanceamento visual entre logotipo e ícones sociais

Tipo: Melhoria
Classificação: Desejabilidade
Prioridade: Baixa

Descrição

No rodapé da página existe um desequilíbrio visual entre:

logotipo posicionado à esquerda

ícones de redes sociais posicionados à direita

O espaçamento entre esses elementos cria uma grande área vazia no centro da tela.

Isso pode transmitir sensação de layout incompleto.

Passos para reproduzir

Acessar o rodapé da página

Observar distribuição dos elementos

Resultado atual

Grande espaço vazio entre logotipo e ícones sociais.

Resultado esperado

Melhor distribuição dos elementos, por exemplo:

centralizar conteúdo

adicionar links institucionais

equilibrar grid do rodapé

BR-016 — [Certificação] Botões com mesmo CTA direcionam para páginas diferentes

Tipo: Correção
Classificação: Usabilidade
Prioridade: Média

Descrição:
Existem dois botões com o mesmo texto “Quero me certificar” na página, porém cada um direciona o usuário para destinos diferentes.

Isso cria inconsistência na navegação e pode gerar confusão no fluxo do usuário, pois ações iguais devem possuir comportamento igual.

Interfaces previsíveis são fundamentais para uma boa experiência do usuário.

Passos para reproduzir:

Acessar a página principal do site

Localizar o botão “Quero me certificar” no topo da página

Clicar no botão

Retornar à página anterior

Localizar outro botão “Quero me certificar” em outra seção da página

Clicar no botão

Resultado atual:
Os botões com o mesmo texto direcionam para páginas diferentes.

Resultado esperado:

Uma das opções deve ser aplicada:

ambos os botões direcionarem para a mesma página, ou

utilizar textos diferentes para cada ação, caso os destinos sejam distintos.

Exemplo:

"Quero me certificar"

"Saiba mais sobre certificação"
