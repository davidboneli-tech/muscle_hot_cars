<div align="center">

# 🏁 Muscle Hot Cars

### Uma garagem digital para uma coleção de verdade.

**📱 Android · 📴 Offline · 🚗 Miniaturas 1:64 · 📸 Catálogo visual**

Um aplicativo pessoal para registrar os detalhes e as fotografias de cada exemplar da coleção.

**6 posições de foto · Backup com imagens · Versão 1.2.0**

</div>

---

## 💡 Por que este aplicativo foi criado?

O Muscle Hot Cars nasceu da minha coleção de carrinhos em escala 1:64 e da vontade de ter um catálogo próprio, simples de usar no celular. Eu queria reunir as informações e as fotos das miniaturas em um lugar só, com acesso mesmo sem internet.

Uma miniatura tem detalhes que merecem registro: o modelo do veículo, a cor, a marca, o fabricante da miniatura, o código e as características visíveis nas fotografias. Dois exemplares parecidos também podem fazer parte da coleção e precisam de cadastros separados.

A aparência fazia parte da proposta desde o início. Eu queria que a ficha do carrinho tivesse personalidade, com inspiração em cartazes de garagem, nome em destaque e uma composição visual ligada ao universo dos muscle cars.

> 🎯 **Objetivo:** facilitar o registro e a consulta da coleção, valorizando a identidade de cada miniatura.

## ✨ O que o aplicativo oferece

| Recurso | Utilidade para o colecionador |
|---|---|
| 🚗 Cadastro por exemplar | Permite registrar miniaturas iguais separadamente |
| 📝 Edição dos dados | Completa ou corrige as informações ao longo do tempo |
| 🔎 Busca e filtros | Ajuda a localizar modelos, marcas, códigos e características |
| 📸 Fotos opcionais | Permite começar um cadastro e fotografar depois |
| 🖼️ Ficha visual | Apresenta o carrinho com identidade de cartaz de garagem |
| 💾 Backup ZIP | Reúne os registros e as fotos salvas em um arquivo |
| ♻️ Restauração | Valida o backup antes de confirmar a importação |
| 📴 Uso offline | Mantém a consulta e os cadastros disponíveis sem rede |

## 🗃️ Cada informação no seu lugar

O cadastro distingue informações que podem parecer iguais, mas representam coisas diferentes:

| Campo | O que representa |
|---|---|
| Modelo | O veículo representado pela miniatura |
| Marca do veículo | A marca do carro real |
| Fabricante da miniatura | A empresa que produziu o carrinho em escala |
| Ano do veículo | O ano atribuído ao modelo representado |
| Ano de lançamento da miniatura | O ano de lançamento daquele produto em escala |
| Código | A identificação do fabricante, preservando letras e zeros iniciais |
| Cor e observações | Características e detalhes do exemplar |

**Somente o modelo é obrigatório.** Os demais dados podem ser preenchidos quando estiverem disponíveis.

## 📸 Seis ângulos para registrar os detalhes

| Posição | O que permite observar |
|---|---|
| 🚘 Frente | Faróis, grade e detalhes frontais |
| 🚙 Traseira | Lanternas e acabamento traseiro |
| 📐 Isométrica | Vista de canto, mostrando mais de uma face |
| ↔️ Lateral | Rodas, pintura e desenho da carroceria — uma única lateral |
| ⬆️ Topo | Teto, capô e detalhes vistos de cima |
| 🔧 Base | Inscrições e características da parte inferior |

Todas as fotos são opcionais. É possível usar a câmera ou selecionar imagens da galeria. As ilustrações dos campos vazios ajudam a identificar a posição e são substituídas quando uma foto real é adicionada.

## 🏎️ Identidade visual

A ficha combina nome do modelo em destaque, faixas, ano e logotipo da marca inclinado, como marca d’água e brasão. A proposta é dar ao catálogo a aparência de uma garagem pessoal, mantendo as informações fáceis de consultar.

A abertura é breve e silenciosa, e existe uma preferência de movimento reduzido. Os recursos visuais devem acompanhar o uso prático do catálogo.

## 💾 Como os dados são preservados

Cada exemplar recebe uma identificação própria, independente do código do fabricante. Os registros ficam em um banco SQLite e as fotos são copiadas para o armazenamento privado do aplicativo.

O backup exporta os dados e as fotos já salvos. Na restauração, o aplicativo valida o arquivo e apresenta uma confirmação antes de mesclar os registros. O arquivo pode ser guardado fora do celular para recuperação futura.

Não existe sincronização automática com a nuvem. Se o usuário escolher um serviço online como destino do arquivo, a conexão depende desse serviço.

## ⚙️ Como foi construído

| Tecnologia | Responsabilidade |
|---|---|
| Java | Integração com câmera, arquivos, armazenamento e backup |
| Android WebView | Executar a interface empacotada no aplicativo |
| HTML + CSS | Organizar as telas e a identidade visual da ficha |
| JavaScript | Cadastros, navegação, busca, filtros e interações |
| SQLite | Armazenar os registros da coleção |
| JPEG + ZIP | Guardar fotografias e reunir o conteúdo dos backups |
| Python | Automatizar a compilação do APK |

A compilação utiliza JDK 17 e Android SDK 35 por meio de script próprio, sem Gradle.

## ✅ Estado do projeto

**Versão documentada: 1.2.0.** O manifesto define Android 8.0 como mínimo. O aplicativo foi pensado para Android e não é exclusivo de um modelo de celular.

Na entrega documentada foram verificadas a compilação, a integridade e a assinatura do APK. Os testes de interface no navegador simulam a integração Android; câmera, seleção de arquivos e restauração precisam de validação no aparelho. Não há comprovação de testes em todos os modelos Android.

## 🤝 Concepção e desenvolvimento

**David dos Santos Boneli** — idealização, definição das necessidades, escolhas de interface, prioridades e avaliação do uso cotidiano.

O desenvolvimento contou com assistência de inteligência artificial na implementação, nas revisões e na documentação. O projeto mostra como uma necessidade pessoal pode ser transformada em requisitos, decisões de produto e um aplicativo funcional, com evolução a partir do uso.

## 📚 Documentação do projeto

| Documento | O que você encontra |
|---|---|
| [Arquitetura](docs/arquitetura.md) | Organização técnica e decisões de implementação |
| [Escopo e validação](docs/escopo_e_validacao.md) | Estado documentado e limites das verificações |
| [Padrão de atualizações](docs/padrao_atualizacoes.md) | Critérios para manter as próximas versões consistentes |
| [Publicação](docs/publicacao.md) | Cuidados com imagens, dados e materiais de terceiros |
| [Histórico](CHANGELOG.md) | Alterações na apresentação do portfólio |
| [Direitos](DIREITOS.md) | Condições de disponibilização |

## 🔐 Sobre este repositório

Esta é a apresentação pública do projeto. O código completo e o instalador permanecem reservados. A publicação da documentação não concede autorização para exploração comercial do aplicativo; consulte o aviso de direitos.

As capturas de tela serão acrescentadas após a revisão dos dados e dos recursos visuais apresentados.
