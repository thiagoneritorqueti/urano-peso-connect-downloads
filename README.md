# Urano Peso Connect — download para Windows

Aplicativo independente para leitura de peso de balança Urano e inserção controlada em um campo de ERP através do cliente de Área de Trabalho Remota (WTS/RDP).

## Baixar o instalador

**[Baixar UranoPesoConnect-Setup-0.1.5-win64.exe](https://github.com/thiagoneritorqueti/urano-peso-connect-downloads/releases/download/v0.1.5/UranoPesoConnect-Setup-0.1.5-win64.exe)**

[Ver arquivos e notas da versão](https://github.com/thiagoneritorqueti/urano-peso-connect-downloads/releases/tag/v0.1.5)

O download é público e não exige conta no GitHub. Compatível com Windows 10/11 x64. O instalador contém Python e bibliotecas do aplicativo; não é necessário instalá-los separadamente.

Inclui interface em português, simulador de pesagem, painel USB/COM, associação do dispositivo, F8 configurável, envio ao campo de texto em foco, com restrição opcional de janela e alternativa por clipboard.

## Usar a tecla de vezes

Na versão 0.1.5, abra **Configurações → Atalho**, selecione **\* (vezes do teclado numérico)** e clique em **Salvar configurações**. Use a tecla de multiplicação no bloco numérico à direita. Clique no campo de destino, pressione e solte a tecla para enviar o peso. Durante o uso desse atalho, o aplicativo consome o asterisco e envia somente o número. Confira o resultado no campo de teste e depois no ERP remoto.

## Início automático e reconexão

O instalador traz marcada a opção **Iniciar o Urano Peso Connect com o Windows e conectar à balança**. Desde a versão 0.1.4, o programa corrige a abertura no login quando um perfil antigo tinha a conexão automática desmarcada. A atualização aproveita o protocolo e a associação USB já salvos. Depois do login na mesma conta, o programa aguarda a balança mesmo se ela estiver desligada. Ao religar ou mudar o cabo para outra tomada USB, deixe um produto parado no prato até aparecer uma nova leitura. Em caso de adaptadores iguais que o programa não consiga distinguir, selecione a COM em **Dispositivos USB**.

## Identificar a comunicação

1. Deixe a balança em **Prot 2**, confirme com **E** e deixe um produto parado no prato.
2. Na aba **Dispositivos USB**, selecione a COM da balança e clique em **Testar todos os protocolos**.
3. O aplicativo testa até 96 combinações de comunicação e reconhece os sete formatos de saída descritos no manual quando chegam pela porta. Quando mostrar três leituras iguais, compare o peso com o visor e clique em **Usar leitura encontrada**.
4. Clique em um campo de texto, no computador ou no ERP remoto, e solte **F8**. Em caso de falha no teste da porta, **Salvar diagnóstico…** exporta as tentativas e os dados recebidos.

## Drivers USB

Se o computador já possui o driver correto, o aplicativo pode ser instalado e utilizado offline. Se o driver estiver ausente, o assistente pode baixar o pacote diretamente da [página oficial da Urano](https://www.urano.com.br/softwares-e-drivers/balancas/). Essa preparação inicial exige internet; a operação de pesagem continua offline. O assistente identifica o hardware antes de oferecer instalação. A instalação de driver pode exigir administrador.

O pacote de drivers não é republicado neste repositório. A edição pública utiliza 7-Zip já instalado ou o extrator do Windows; se o sistema não conseguir abrir o RAR oficial, o assistente informa a necessidade de atualizar/instalar o 7-Zip. Dispositivos sem INF correspondente precisam do instalador específico do fabricante.

## Validar antes do uso

Versão candidata à homologação. Testes automatizados e compilação Windows não substituem o teste com balança física e ERP/WTS real. Comece pelo simulador e pelo campo local de teste; depois confirme identificação USB, driver, parâmetros seriais, tara, estabilidade e F8 em janela/tela cheia. O manual completo acompanha o instalador.

Este repositório hospeda os downloads. O repositório de desenvolvimento é privado. Projeto independente, sem vínculo com a Urano.
