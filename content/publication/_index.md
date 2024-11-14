---
title: Publications
cms_exclude: true

# View.
view: citation

# Optional header image (relative to `static/media/` folder).
banner:
  caption: ''
  image: ''

{{ range .Pages }}
{{ $index := add .Site.Params.publicationCount 1 }} <!-- The index number starts from 1 -->
- **{{ $index }}. [{{ .Title }}]({{ .Permalink }})**  
  {{ .Params.authors }} ({{ .Params.year }})
{{ end }}
---
