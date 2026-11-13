# 🛠️ Desenvolvimento e distribuição

**Versão:** v0.4 RC • **Status:** candidata a lançamento.

O programa é uma aplicação desktop em Python com interface gráfica, compilada em um executável único para Windows 64 bits com PyInstaller. O jogador final **não precisa instalar Python**.

O mecanismo trata dados de saves `ScsC`, `BSII` e `SiiN`. A gravação é limitada a formatos editáveis compatíveis com SiiN e exige backup.

## Como distribuímos

O instalador tradicional não é necessário: basta executar o `.exe`. O arquivo oficial será anexado na seção [Releases](https://github.com/CavernaDoTorresmo/CavernaDoTorresmo_SaveEditor/releases), junto ao SHA-256.

Antes de anunciar a v1.0, a recomendação é verificar a restauração de backup e realizar testes em outro PC Windows sem Python, além de diferentes saves ETS2/ATS.

## Sobre o código-fonte

O código-fonte do projeto não está necessariamente publicado apenas porque o executável está distribuído. Para compilação independente e revisão pública, deverão ser adicionados o código e os recursos de `app.py`, `model.py`, `codec.py`, a pasta `assets`, os testes, o arquivo de requisitos e o script de compilação.

**Licença:** ainda não foi escolhida uma licença aberta para este projeto. Não presumimos licença de terceiros nem declaramos direitos não confirmados. Antes de disponibilizar o código para reutilização, definir uma licença e revisar as atribuições necessárias.

[⬅️ Voltar ao início](../README.md)
