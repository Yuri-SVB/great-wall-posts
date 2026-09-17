# Posts — what's coming, and how this is laid out

The feed itself is in the [repository README](../README.md).

## Coming

| Post | Languages planned |
|---|---|
| The (F/W)rench Attack | en · pt-BR · fr · it |
| Gold With Extra Steps | en · pt-BR |
| Obscurity, the Clearest Problem Nobody Talks About | en · pt-BR · fr · it |
| The Deadly Race | en |
| They Only Took My Pokémon Cards | en · sv |
| The Balland Case — an Embarrassment to the Self-Custody Creed | en · fr |
| Anosognosia | en |

## Layout

```
posts/NNN-kebab-case-title/
    en.md  pt-BR.md  fr.md  it.md      one file per language, IETF tag
    assets/                            figures, embedded by every edition
```

`NNN` is a stable identifier, not a position — the order of the feed changes, the
directory names do not.
