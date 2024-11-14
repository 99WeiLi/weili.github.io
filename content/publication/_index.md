---
1. title: Publications
cms_exclude: true

# View.
view: citation

# Optional header image (relative to `static/media/` folder).
banner:
  caption: ''
  image: ''

## Publications

{{ range .Pages }}
  {{ $index := add 1 (index .Params "number" 0) }}  <!-- Extracts the 'number' and starts from 1 -->
  - **{{ $index }}.** [{{ .Title }}]({{ .Permalink }})  
    **Authors**: {{ .Params.authors }}  
    **Year**: {{ .Params.year }}  
{{ end }}
---
