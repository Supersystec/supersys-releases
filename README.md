# supersys-releases

Repositorio PUBLICO de artefatos de release e feed de auto-update (Velopack) dos projetos Supersystec. O codigo-fonte de cada projeto e privado.

## Convencao por projeto

GitHub Releases nao tem pastas — a separacao por projeto e feita por **channel do Velopack** e **prefixo de tag**:

| Projeto | Channel Velopack | Prefixo de tag | Exemplo de release |
|---|---|---|---|
| SuperTools | `supertools-win` | `supertools-v` | `supertools-v2026.710.1959` |
| SuperTools (beta) | `supertools-win-beta` | `supertools-beta-v` | `supertools-beta-v2026.711.530` (prerelease) |

- Cada release contem os assets do Velopack do projeto: `Setup.exe` (renomeado `<Projeto>Setup.exe`), `*-full.nupkg`, `*-delta.nupkg` e `releases.<channel>.json`.
- O app cliente aponta `GithubSource` para este repo com `ExplicitChannel = <channel>` — releases de outros projetos sao ignorados automaticamente.
- Projeto novo = nova linha nesta tabela + channel/tag proprios. Nunca publicar sem prefixo de tag (colide com outros projetos).

