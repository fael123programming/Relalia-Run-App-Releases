# Relalia Run App — Downloads

Repositório público de distribuição do **Relalia Run App** para **Windows x64**. Contém somente uma página de orientação e releases com instaladores, notas de versão e arquivos de integridade. O código-fonte e seu histórico permanecem privados.

## Baixar

- [Versão mais recente](https://github.com/fael123programming/Relalia-Run-App-Releases/releases/latest)
- [Todas as versões](https://github.com/fael123programming/Relalia-Run-App-Releases/releases)

Abra a versão desejada e, em **Assets**, baixe o arquivo `Relalia-Run-App-<versão>-Setup.exe`. Os downloads são públicos e não exigem conta no GitHub.

## Arquivos de cada versão

- `Setup.exe`: instalador do aplicativo.
- `Setup.exe.sha256`: hash para conferir a integridade do instalador.
- `Setup.exe.blockmap` e `latest.yml`: metadados de distribuição.

No PowerShell, use `Get-FileHash .\Relalia-Run-App-<versão>-Setup.exe -Algorithm SHA256` e compare com o arquivo `.sha256`.

## Instalação e atualização

Feche o aplicativo antes de executar o instalador e preserve um backup dos seus dados. Consulte as notas da versão para verificar compatibilidade e limitações. Os instaladores atuais não têm assinatura Authenticode; hashes verificam integridade, sem substituir a assinatura do fabricante.

A partir da **3.0.4**, o botão **Verificar atualizações** consulta este repositório público. Consulta e download não exigem login, token ou GitHub CLI. O download é solicitado pelo usuário; reinício e instalação continuam explícitos, após concluir as gravações.

As versões até a **3.0.3** ainda usam o canal privado original. Para adotar o canal público, baixe e execute o instalador **3.0.4** uma vez. Quem tem acesso ao canal privado também pode receber essa versão de transição pelo botão antigo. Depois da instalação, as próximas consultas usarão o canal público.

As notas históricas podem mencionar a distribuição privada e documentação técnica interna; elas descrevem o contexto original de cada versão. Este repositório não publica o código-fonte.
