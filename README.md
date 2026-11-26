# Cartão de visita · FHE POUPEX

Página de geração de cartão de visita publicada pelo GitHub Pages, usando o fundo texturizado, a marca FHE POUPEX e os elementos gráficos fornecidos pelo usuário.

## Usar

Preencha nome, cargo, setor, e-mail e telefone. O cartão e o QR Code são atualizados automaticamente. Escolha **Baixar PDF** ou **Salvar contato** para baixar o arquivo correspondente. O botão **Usar exemplo** preenche dados fictícios para avaliação.

A página processa os dados e gera os arquivos no navegador, sem enviar os contatos a um servidor.

## Carteiras digitais

Apple Wallet e Google Wallet estão em preparação: exigem contas de emissão e credenciais institucionais, além de um servidor de emissão. GitHub Pages hospeda apenas a parte estática e não executa esse servidor. Os botões informam a pendência e não simulam a emissão de passes.

O arquivo [projeto-completo.zip](projeto-completo.zip) contém a versão modular da aplicação, o servidor de emissão, testes e instruções de configuração para a equipe de TI. Nenhuma senha, chave privada ou credencial institucional está incluída.

Para a Apple, solicitar Apple Developer institucional, Team ID, Pass Type ID, certificado de assinatura, chave privada e certificado intermediário WWDR. Para o Google, solicitar Issuer ID, conta de serviço autorizada no console Google Wallet, credencial no servidor e endereço HTTPS público da marca. As instruções completas estão no README dentro do ZIP.

## Publicação

Configurar **Settings → Pages → Deploy from a branch → main → /(root)**. O arquivo `index.html` contém a interface, estilos, marca e bibliotecas locais, sem dependências externas. A aparência nas carteiras depende de cada plataforma e deve ser homologada em aparelhos reais.

## Validação

A interface foi conferida em telas de computador e celular. PDF e vCard foram baixados pela interface e inspecionados; a aplicação modular passou em 14 testes. Os testes de Apple usaram certificado de teste e os de Google usaram respostas simuladas. A emissão nas carteiras reais depende das credenciais e da homologação institucional.

## Atribuições

Evolução do estudo de layout original deste repositório, preservado no histórico. QRCode for JavaScript: Kazuhiko Arase, licenças e avisos Apache 2.0 / MIT preservados no HTML. pdf-lib: MIT, licença também incluída no projeto completo. Marcas de seus respectivos titulares. Esta publicação não representa homologação institucional.
