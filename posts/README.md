# Posts — what's coming, and how this is laid out

The feed itself is in the [repository README](../README.md).

## Coming

Every post ships in English, Portuguese, Spanish, French and Italian; there is no
per-post language plan. The ten posts that have run are in the
[repository README](../README.md).

- Hot Takeaways of the Coldcard Hack *(written, English only; cover pending)*
- A Prediction, Dated and Signed *(written, English only; cover pending)*

A Swedish edition of They Only Took My Pokémon Cards is planned and needs a
human translator. The Balland Case is running with a placeholder cover.

## Layout

```
posts/NNN-kebab-case-title/
    en.md  pt-BR.md  es.md  fr.md  it.md    one file per language, IETF tag
    assets/                            figures, embedded by every edition
```

`NNN` is a stable identifier, not a position — the order of the feed changes, the
directory names do not.
