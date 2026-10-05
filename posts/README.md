# Posts — what's coming, and how this is laid out

The feed itself is in the [repository README](../README.md).

## Coming

In publication order. Every post ships in English, Portuguese, Spanish, French
and Italian; there is no per-post language plan.

- The (F/W)rench Attack *(written)*
- From Magic Internet Money to Gold With Extra Steps
- Obscurity, the Clearest Problem Nobody Talks About *(written)*
- The Deadly Race *(written)*
- They Only Took My Pokémon Cards *(written; a Swedish edition is planned and needs a human translator)*
- Bloodshed *(written)*
- The Balland Case — an Embarrassment to the Self-Custody Creed *(written; cover pending)*
- Anosognosia *(written; cover pending)*

## Layout

```
posts/NNN-kebab-case-title/
    en.md  pt-BR.md  es.md  fr.md  it.md    one file per language, IETF tag
    assets/                            figures, embedded by every edition
```

`NNN` is a stable identifier, not a position — the order of the feed changes, the
directory names do not.
