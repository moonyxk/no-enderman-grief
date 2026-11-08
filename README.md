# No Enderman Grief

Ein Paper-Plugin für Minecraft Java Edition 26.3. Es verhindert, dass
Endermen Blöcke aufheben. Das Ablegen bereits getragener Blöcke bleibt erlaubt.

![Enderman hebt keinen Block auf](https://cdn.modrinth.com/data/cached_images/d71ea7955e7bacbd8307c87c4bc9101a2d903c75.png)

## Voraussetzungen

- Java 25 oder neuer
- Paper 26.3

## Bauen

Unter Windows:

```powershell
.\gradlew.bat build
```

Unter Linux/macOS:

```sh
./gradlew build
```

Das Plugin-JAR liegt anschließend in `build/libs/`. Kopiere es in den
`plugins/`-Ordner deines Paper-Servers und starte den Server neu.

## Verhalten

Das Plugin bricht nur Änderungen ab, bei denen ein Enderman einen vorhandenen
Block in Luft verwandeln würde. Andere Entitäten und das Platzieren eines
getragenen Blocks bleiben unverändert.
