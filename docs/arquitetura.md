# Arquitetura — Muscle Hot Cars

## Organização do aplicativo reservado

| Local | Responsabilidade |
|---|---|
| app/src/main/java/ | Código de integração com o Android |
| app/src/main/assets/ | HTML, CSS, JavaScript, conteúdo e recursos locais |
| app/src/main/res/ | Ícones, temas e recursos Android |
| app/src/main/AndroidManifest.xml | Identificação e componentes do aplicativo |
| tools/ | Scripts de preparação, compilação e verificações |

Esses caminhos descrevem o projeto completo reservado; não são pastas de código deste repositório público.

## Funcionamento

O Android abre uma WebView que carrega a interface empacotada no próprio APK. HTML e CSS apresentam as telas; JavaScript trata as interações e usa a ponte nativa quando necessário. O manifesto não solicita permissão de internet.

Uma camada Java mantém os registros em SQLite e as fotos JPEG no armazenamento privado do aplicativo. Cada exemplar recebe um UUID independente do código do fabricante. Backups ZIP incluem registros e fotos.

## Decisões

- Identificação por UUID para permitir miniaturas iguais em cadastros separados.
- Fotos opcionais para permitir um cadastro rápido e preenchimento posterior.
- Validação do backup e confirmação antes da restauração.

## Compilação

O projeto completo possui script Python próprio, utilizando JDK 17, Android SDK Platform 35 e Build Tools 35.0.0, sem Gradle. O repositório público é documental e não permite compilar o aplicativo.
