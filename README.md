# output-codeql-db

Prepare a CodeQL database for extraction.

### Example

```yaml
- id: output-codeql-db
  uses: mario-campos/output-codeql-db@main
  with:
    language: javascript
- uses: actions/upload-artifact@v2
  with:
    path: ${{ steps.output-codeql-db.outputs.path }}
```
