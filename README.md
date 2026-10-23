# Galleria — Portal do Cliente

Protótipo mobile da jornada de assinatura, com identidade Galleria e três etapas: biometria, fichas cadastrais e contrato/CCI.

## Ativar o navegável

No GitHub: **Settings → Pages → Deploy from a branch → main → / (root) → Save**.

Após a publicação, o GitHub exibirá o endereço do site nessa mesma tela. Compartilhe o link do site com o time para navegar sem instalar nada.

## O que testar

A abertura acontece após a assinatura das fichas, com **2 de 3 etapas concluídas** e a CCI pendente. Clique em **Continuar para a última etapa**. Os atalhos no rodapé permitem testar todas as etapas.

A confirmação geral só aparece depois da confirmação simulada da CCI. O retorno do aplicativo do certificado, por si só, mantém a etapa pendente.

## Arquivos

- `index.html`: interface, estilos e navegação.
- `assets/galleria-logo.png`: logo fornecido para o projeto.
- `.nojekyll`: publicação estática sem processamento Jekyll.

Abra `index.html` no navegador para executar localmente. Não é necessário instalar dependências.

## Escopo

Demonstração com dados fictícios, sem captura de biometria, assinatura real, emissão de boletos ou integração financeira. Nenhum vídeo, dado de cliente ou credencial foi incluído no repositório. A integração real exige backend e confirmação dos provedores.
