# 🛡️ Segurança e boas práticas

Este é um editor de saves **não oficial** em versão candidata a lançamento (**v0.4 RC**).

## Antes da edição

- Feche completamente ETS2/ATS.
- Faça backup da **pasta inteira do perfil** (não apenas de um arquivo).
- Use um salvamento **manual**, recém-criado, e identifique a pasta correta.
- Evite sincronizar versões diferentes pela Steam Cloud durante o teste.
- Não execute o editor como administrador se não houver necessidade.

## Proteção dos dados

O aplicativo foi projetado para operar localmente, sem cadastro nem telemetria. O arquivo `game.sii` contém informações de progresso; **nunca envie seu save completo em issues públicas**. O caminho do Windows pode revelar o nome do usuário; oculte essas informações em capturas.

O editor produz um `.bak` antes de gravar, mas mantenha também um backup externo da pasta do perfil.

## Download e verificação do SHA-256

A soma do arquivo oficial `CavernaDoTorresmo_SaveEditor.exe` da versão 0.4 RC deve ser:

```text
B3DFD83DAD8B54DFD01C8BA330B11B48FAACD03D052104F8663AB32A8232C6BF
```

No PowerShell:

```powershell
Get-FileHash .\CavernaDoTorresmo_SaveEditor.exe -Algorithm SHA256
```

A comparação verifica a integridade do arquivo em relação ao release, **não garante ausência de malware**. O executável não possui assinatura digital e o Windows SmartScreen pode avisar sobre baixa reputação. **Não desative antivírus ou SmartScreen para executar.** Execute apenas se tiver confiança na origem e no arquivo.

## Se o save ficar incorreto

1. Feche o jogo imediatamente.
2. Faça cópia do arquivo editado para diagnóstico privado.
3. Localize o backup `.bak` gerado.
4. Restaure o `game.sii` original.
5. Se necessário, restaure a pasta inteira do perfil.

## Limitações conhecidas

- Suporte de escrita limitado a formatos compatíveis com SiiN (direto ou ScsC).
- Saves BSII podem ser lidos, mas não gravados.
- Coaches validado em um perfil ETS2; outras combinações de versão/mods não foram totalmente testadas.
- Edição de garagens é experimental.

Não afiliado à SCS Software.

[⬅️ Voltar ao início](../README.md)
