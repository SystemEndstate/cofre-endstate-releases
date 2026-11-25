# Cofre Endstate · releases

Este repositório guarda **só as versões publicadas** do Cofre Endstate, o cofre de senhas portátil da Endstate. Ele não tem código-fonte nem dado de ninguém.

Cada release traz quatro arquivos:

| Arquivo | O que é |
|---|---|
| `CofreEndstate.exe` | o programa |
| `CofreEndstate.exe.sha256` | o hash SHA-256 do programa |
| `CofreEndstate.exe.sig` | a assinatura Ed25519 da Endstate sobre a versão e o hash |
| `release.json` | versão, novidades e hash |

O Cofre se atualiza sozinho a partir daqui. Ele só instala uma versão nova quando a assinatura confere com a chave pública embutida no programa **e** o hash bate. Antes de trocar o programa, faz uma cópia da pasta `dados`. Se a versão nova não abrir, volta sozinho para a anterior.

A verificação lê só esta página pública. Nenhuma informação do cofre sai do pendrive.

© 2026 Endstate
