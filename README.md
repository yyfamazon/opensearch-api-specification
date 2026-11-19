# Bundled spec: before and after

Only the bundled `opensearch-openapi.yaml` (`npm run merge`), so the changes to the published file can be reviewed on their own. Compare the commits:

1. `main` (`de8c154`).
2. With opensearch-project/opensearch-api-specification#1291: properties declared next to `allOf`/`oneOf`/`anyOf` moved into an `allOf` member (`TermsLookup`, `SemanticProperty`), and every union labeled with `x-union-kind` (plus `x-variant-keys` for containers).
3. With the generic-instantiation labels on top: `x-type-arguments` on every `allOf: [ $ref Generic, {...} ]`.
