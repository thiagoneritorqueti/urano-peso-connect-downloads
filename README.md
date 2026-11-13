# Urano Peso Connect — download para Windows

Aplicativo independente para leitura de peso de balança Urano e inserção controlada em um campo de ERP através do cliente de Área de Trabalho Remota (WTS/RDP).

## Baixar o instalador

**[Baixar UranoPesoConnect-Setup-0.1.1-win64.exe](https://github.com/thiagoneritorqueti/urano-peso-connect-downloads/releases/download/v0.1.1/UranoPesoConnect-Setup-0.1.1-win64.exe)**

[Ver arquivos e notas da versão](https://github.com/thiagoneritorqueti/urano-peso-connect-downloads/releases/tag/v0.1.1)

O download é público e não exige conta no GitHub. Compatível com Windows 10/11 x64. O instalador contém Python e bibliotecas do aplicativo; não é necessário instalá-los separadamente.

Inclui interface em português, simulador de pesagem, painel USB/COM, associação do dispositivo, F8 configurável, autorização da janela de destino e alternativa por clipboard.

## Drivers USB

Se o computador já possui o driver correto, o aplicativo pode ser instalado e utilizado offline. Se o driver estiver ausente, o assistente pode baixar o pacote diretamente da [página oficial da Urano](https://www.urano.com.br/softwares-e-drivers/balancas/). Essa preparação inicial exige internet; a operação de pesagem continua offline. O assistente identifica o hardware antes de oferecer instalação. A instalação de driver pode exigir administrador.

O pacote de drivers não é republicado neste repositório. A edição pública utiliza 7-Zip já instalado ou o extrator do Windows; se o sistema não conseguir abrir o RAR oficial, o assistente informa a necessidade de atualizar/instalar o 7-Zip. Dispositivos sem INF correspondente precisam do instalador específico do fabricante.

## Validar antes do uso

Versão candidata à homologação. Testes automatizados e compilação Windows não substituem o teste com balança física e ERP/WTS real. Comece pelo simulador e pelo campo local de teste; depois confirme identificação USB, driver, parâmetros seriais, tara, estabilidade e F8 em janela/tela cheia. O manual completo acompanha o instalador.

Este repositório hospeda os downloads. O repositório de desenvolvimento é privado. Projeto independente, sem vínculo com a Urano.
