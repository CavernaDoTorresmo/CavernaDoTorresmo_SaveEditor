# 🚌 Como usar — Caverna do Torresmo Save Editor

**Versão:** 0.4 RC • **Sistema:** Windows 10/11 (64 bits) • **Idioma:** português

## 1. Prepare um save seguro

1. Abra o ETS2 ou ATS.
2. Se pretende editar a DLC **Coaches**, complete ao menos uma viagem de ônibus para inicializar a progressão.
3. Crie um **salvamento manual**.
4. Feche completamente o jogo.
5. Faça uma cópia de segurança da **pasta inteira do perfil** antes de editar.

Locais comuns:

```text
Documentos\Euro Truck Simulator 2\profiles\<id_do_perfil>\save\<pasta_do_save>\game.sii
Documentos\American Truck Simulator\profiles\<id_do_perfil>\save\<pasta_do_save>\game.sii
```

Se usa Steam Cloud, o perfil pode aparecer em `steam_profiles`. Prefira o salvamento manual correto, não o autosave.

## 2. Abra o editor

Inicie `CavernaDoTorresmo_SaveEditor.exe` pelo Windows, sem precisar instalar Python.

Clique em **Detectar saves** ou **Abrir game.sii** e escolha o arquivo. Os valores disponíveis aparecerão nas respectivas seções.

## 3. Ajuste o que precisa

Na seção **Coaches — Ônibus**, altere XP de ônibus e as seis habilidades. O botão **Maximizar as 6 habilidades** define os atributos no máximo; a opção **3/3 + copiar XP** também usa o XP do caminhoneiro como referência. O nível de ônibus é calculado pelo jogo, portanto pode variar.

Outras abas incluem **Perfil e dinheiro**, **Caminhão** e **Garagens** (experimental). Não altere valores cujo efeito você não compreende.

## 4. Revise e salve

Revise as mudanças exibidas no programa e clique em **Salvar com backup**. O editor cria um arquivo `.bak` na mesma pasta antes de substituir o save. Depois abra o jogo e carregue **o mesmo salvamento manual**.

## Meu arquivo é somente leitura / BSII

Alguns saves usam `BSII` binário e não podem ser gravados por esta versão. Feche o jogo e abra o arquivo `config.cfg` da pasta principal do ETS2/ATS. Localize:

```text
uset g_save_format "2"
```

Se o valor for diferente, ajuste para `"2"`, salve o `config.cfg`, entre no jogo e **crie um novo salvamento manual**. Depois feche o jogo e abra o novo `game.sii` no editor. O formato editável esperado é **ScsC + SiiN** (ou texto SiiN).

## Como voltar atrás

1. Feche o jogo.
2. Localize o `game.sii.DATA_HORA.bak` da edição.
3. Guarde o `game.sii` editado em outro lugar.
4. Copie o backup e renomeie a cópia para `game.sii`.
5. Abra o ETS2/ATS e carregue o salvamento.

Se a Steam Cloud sincronizar uma versão diferente, compare os saves antes de continuar. Consulte [SEGURANCA.md](SEGURANCA.md).

---

[⬅️ Voltar ao início](../README.md)
