# output-codeql-db

Get the path of the CodeQL database for uploading as an artifact.

### Example

```yaml
- id: output-codeql-db
  uses: mario-campos/output-codeql-db@main
  with:
    language: javascript
- uses: actions/upload-artifact@v2
  with:
    name: codeql-db.zip
    path: ${{ steps.output-codeql-db.outputs.path }}
```
