# [tools.json](https://cecekpawon.github.io/revanced-extended-tools-api/tools.json)
Auto update `Revanced Extended` Tools API like official https://releases.revanced.app/tools

``1
curl -s https://cecekpawon.github.io/revanced-extended-tools-api/tools.json | \
  jq -r  '.[] | map(select(.label == "patches_jar"))[] | .version'
```