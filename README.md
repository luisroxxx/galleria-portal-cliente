# Galleria — Portal do Cliente

Demonstração mobile completa da experiência de acesso, assinatura e pós-contrato.

## Navegável

https://luisroxxx.github.io/galleria-portal-cliente/

## Como testar

1. Na entrada, utilize o CPF demonstrativo **000.000.000-00**, selecione o cartão **SMS, WhatsApp ou E-mail** e clique em **Receber código**. O destino é sempre o contato previamente cadastrado, sem campo para informar telefone ou e-mail.
2. Use o código **123456** ou o botão de preenchimento de exemplo.
3. Abra o contrato e confira o resumo da proposta fictícia.
4. Inicie a biometria simulada: orientações, ilustração de enquadramento, processamento e confirmação.
5. Abra as três fichas e confirme a leitura de cada uma. Marque o aceite demonstrativo e clique em **Assinar fichas cadastrais** na mesma tela.
6. Confira a tela **2 de 3 concluídas**: a CCI continua pendente.
7. Leia a CCI já aberta e siga para o certificado, sem checkbox adicional.
8. Com a CCI visível, selecione **VIDaaS** abaixo do documento e simule a autorização no modal da própria tela. Clique em **Voltar ao Galleria e confirmar**.
9. Aguarde a confirmação da CCI para visualizar **3 de 3 etapas concluídas**.
10. Acompanhe a operação e, opcionalmente, clique em **Simular contrato ativo** para explorar pagamentos, parcelas e antecipação.

## Situações adicionais

- **Testar cenários** no rodapé: falha na próxima biometria, cancelamento no certificado e demora na confirmação da CCI.
- **Salvar e continuar depois**, saída e recarga: o progresso fictício é salvo no mesmo navegador. O acesso é reiniciado e a jornada retoma a partir das etapas confirmadas.
- Na demora da CCI, use **Consultar novamente**. A primeira consulta adicional mantém a pendência; a seguinte simula confirmação.
- **Reiniciar jornada** apaga somente o progresso desta demonstração.
- O resumo de assinatura pode ser baixado como TXT demonstrativo.

## Escopo e limites

Não há autenticação real, envio de SMS, WhatsApp ou e-mail, acesso à câmera, prova de vida real, assinatura com validade jurídica, emissão de boleto ou transação financeira. Utilize apenas o CPF fictício 000.000.000-00 e o código 123456. Não forneça dados pessoais reais.

Contratos, documentos, valores e datas são fictícios. A área de antecipação permite simular a solicitação de cotação; não calcula desconto, saldo, novo prazo ou nova parcela. O boleto demonstrativo não possui código de pagamento.

Os estados ficam no localStorage apenas para testar retomada. Em produção, a fonte de verdade deve ser o backend, com autenticação, autorização por operação e confirmação idempotente dos provedores. O retorno do certificado não equivale à assinatura do documento.

## Arquivos e execução

- `index.html`: interface, estilos e navegação sem dependências externas.
- `assets/galleria-logo.png`: logo fornecido pelo usuário, somente Galleria.
- `.nojekyll`: publicação estática.

Abra `index.html` em um navegador, ou sirva a pasta localmente. GitHub Pages está configurado para a branch `main`, pasta raiz.

## Validação desta versão

Verificados no navegador: entrada e código de exemplo; proposta; biometria; bloqueio por documentos não lidos; leitura das três fichas; assinatura parcial; saída e retomada; leitura da CCI; cancelamento e nova tentativa no certificado; retorno e confirmação final; acompanhamento e ativação fictícia; valor de antecipação inválido e cenário válido.
