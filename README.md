# Pocket Bullet Lab — builds de teste

Este repositório contém **apenas os APKs de teste** do Pocket Bullet Lab, publicados como releases. O código-fonte fica em um repositório privado.

## Instalar e atualizar no Android

1. Instale o [Obtainium](https://github.com/ImranR98/Obtainium/releases/latest) (`app-arm64-v8a-release.apk`).
2. No Obtainium, use **Adicionar app** com `https://github.com/RafaelBritoChoco/pocket-bullet-lab-builds`.
3. Abra o Obtainium quando quiser e toque em **Atualizar** se houver versão nova.

Os APKs são assinados sempre com a mesma chave, então as atualizações mantêm o progresso salvo.

## Para quem publica

Não envie arquivos manualmente aqui. As versões chegam de dois jeitos:

- **Automático (padrão):** todo push em `main` ou `round/**` no repositório do jogo roda o GitHub Actions, que gera o APK e o envia para a branch `incoming` daqui; o workflow `release-incoming.yml` cria o release. Funciona com o PC desligado.
- **Pelo PC:** `scripts/release/update-android.ps1 -ExportOnly -Publish`.

Veja `docs/RELEASING.md` no repositório do jogo.

## Créditos

Sprites do Sunnyside World Asset Pack (Daniel Diggle). Os assets não são redistribuídos separadamente: este repositório contém só o jogo compilado.
