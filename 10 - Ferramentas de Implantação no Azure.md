# Ferramentas de Implantação no Azure

## Objetivo
Apresentar as principais ferramentas de implantação no Azure, destacando o uso do Cloud Shell, a automação via Bash/PowerShell e a linguagem Bicep.

### Cloud Shell no Azure

O Azure Cloud Shell é uma ferramenta que você pode usar diretamente no navegador para gerenciar seus recursos no Azure.

- Acesso Fácil: Você pode acessar e gerenciar seus recursos do Azure de qualquer lugar, sem precisar instalar nada.
- Escolha de Shell: Pode usar comandos do Bash ou do PowerShell, conforme sua preferência.
- Ferramentas Prontas: Já vem com várias ferramentas e linguagens de programação instaladas.
- Armazenamento Seguro: Seus arquivos são salvos e mantidos seguros entre as sessões.
- Editor de Arquivos: Tem um editor de arquivos integrado para criar e editar arquivos diretamente.

### Para acessar o Cloud Shell
- No canto superior direito clique em "Cloud Shell" abrirá em Bash
- ![alt text](<cloud shell1-1.PNG>)
- Em *"Switch to Power Shell"* troca para o Power Shell 
![alt text](<cloud shell2.PNG>)
- Em *"Manage Files"* pode fazer upload e download de arquivos.
- ![alt text](<cloud shell3.PNG>) 

- Versão Bash - Interface Preta
![alt text](<cloud shell4.PNG>)
- Versão Power Shell - Interface Azul
![alt text](<cloud shell5.PNG>)

*" Podemos acessar o azure via comando usando *"Bash ou PowerShell"* através da sua Maquina Local é possivel desde que esteja instalado os modulos do Azure nela.

### Automation (Automação)

#### Via Bash/PowerShell

"Implementar um recurso qualquer manualmente no azure" Ex: Virtual Machine | Vnet
- Na aba *"Automation"* em Vnet temos:
  - CLI/PS : Mostra alguns comandos de implementação de uma Vnet para serem executados via comando *"Bash ou PowerShell"*
  - ![alt text](CLI.PNG)
  - ![alt text](PS.PNG)
- Export Template :  Mostra o arquivo (Template) no formato JSON para salvar em nossa maquina local e re-utilizar no futuro o mesmo recurso configurado , quando necessário. Pode ser implementado via comando no **"Bash ou power shell"** no Cloud Shell
  -  ![alt text](<EXPORT TEMPLATE.PNG>)

    
- Ao salvar o arquivo na Maquina Local temos o arquivo Template.JSON e Parameters.JSON , o Template é o recurso em comando e o Parameters é usado para alterar o template.
  - ![alt text](arquivos.PNG)

## Conclusão

O Azure Cloud Shell permite gerenciar recursos diretamente do navegador, com suporte para Bash e PowerShell, além de ferramentas integradas e armazenamento seguro. A aba Automation simplifica a criação de recursos, fornecendo comandos prontos e templates exportáveis para reutilização.

O Bicep surge como uma linguagem mais simples e legível para definir e implantar recursos no Azure, oferecendo suporte completo e integração com ferramentas de desenvolvimento como o Visual Studio Code.

Essas ferramentas e práticas ajudam a otimizar o gerenciamento de recursos no Azure, proporcionando uma experiência mais fluida e produtiva para desenvolvedores e administradores.