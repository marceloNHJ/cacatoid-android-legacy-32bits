# Cacatoid Android Legacy 32-bit

Fork não oficial do projeto
[`lmajowka/cacatoid`](https://github.com/lmajowka/cacatoid).

Esta versão foi criada para tentar executar o projeto em dispositivos Android
mais antigos com arquitetura ARM de 32 bits.

> [!WARNING]
> Este fork foi criado para uma necessidade específica e não é uma versão
> oficial do projeto original.

> [!IMPORTANT]
> Não ofereço manutenção, suporte técnico, correções, atualizações ou
> garantia de funcionamento. Qualquer uso, instalação ou modificação é de
> responsabilidade do usuário.

> [!NOTE]
> A adaptação foi realizada com auxílio de inteligência artificial para
> orientação técnica e solução de problemas de compilação. As alterações
> foram feitas e testadas pelo autor em um dispositivo real.

## Dispositivo de referência

O fork foi compilado, instalado e aberto com sucesso em:

| Item | Informação |
|---|---|
| Modelo | Samsung Galaxy J4 Core |
| Sistema | Android 8.1 Oreo |
| API | 27 |
| Processador | ARM Cortex-A53 |
| ABI | `armeabi-v7a` |

Esse teste confirma o funcionamento nesse dispositivo específico. Não confirma
compatibilidade com todos os aparelhos que tenham especificações semelhantes.

## Características da versão

Esta variante foi configurada para:

- Android API 27 ou superior;
- dispositivos ARM de 32 bits;
- ABI `armeabi-v7a`.

O APK compilado pode ser disponibilizado na página de
[Releases](../../releases).

A existência de um APK nesta página não representa garantia de suporte ou de
funcionamento em outros dispositivos.

## Modificações principais

As principais alterações em relação ao projeto original foram:

- `minSdk` ajustado de 28 para 27;
- ABI nativa alterada para `armeabi-v7a`;
- remoção das ABIs `arm64-v8a` e `x86_64` desta variante;
- substituição de `unsigned __int128`;
- uso de `boost::multiprecision::uint128_t`;
- recompilação da biblioteca nativa para ARM de 32 bits.

Essas mudanças foram feitas especificamente para permitir a compilação e o
funcionamento no dispositivo de referência.

## Estado do projeto

Este é um fork experimental e sem manutenção planejada.

Não há compromisso de:

- acompanhar atualizações do projeto original;
- corrigir problemas relatados por terceiros;
- adaptar o APK para outros modelos;
- publicar novas versões;
- oferecer ajuda com instalação ou configuração.

Se algo funcionar em outro aparelho, isso será uma consequência não testada,
não uma garantia de compatibilidade.

## Forks e modificações

Quem quiser tentar adaptar o projeto para outro dispositivo ou versão do
Android pode:

- criar um fork deste repositório;
- alterar as configurações de compilação;
- modificar o código nativo;
- gerar uma nova versão do APK;
- usar o projeto original como ponto de partida.

As modificações de terceiros não são mantidas nem supervisionadas neste
repositório. Qualquer redistribuição deve respeitar as licenças aplicáveis.

## Projeto original

O código original está disponível em:

<https://github.com/lmajowka/cacatoid>

Este repositório não substitui o projeto original e pode ficar desatualizado
em relação a ele.

## Créditos e licenças

Os créditos, avisos de copyright e arquivos de licença do projeto original e
de suas dependências devem ser preservados.

Antes de redistribuir o código ou o APK, verifique os termos da licença do
projeto original e de todos os componentes utilizados.

Este fork não concede direitos adicionais sobre o código original ou sobre
suas dependências.
