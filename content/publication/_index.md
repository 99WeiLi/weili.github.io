---
1. title: Publications
cms_exclude: true

# View.
view: citation

# Optional header image (relative to `static/media/` folder).
banner:
  caption: ''
  image: ''
---
## Publications

{{ range .Pages }}
  - **{{ .Loop.Index }}.** [{{ .Title }}]({{ .Permalink }})  
    **Authors**: {{ .Params.authors | join ", " }}  
    **Year**: {{ .Params.date | date "2006" }}  
    **DOI**: [{{ .Params.doi }}](https://doi.org/{{ .Params.doi }})
{{ end }}