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
{{ range .Pages }}
  - **{{ .PageCount }}.** [{{ .Title }}]({{ .Permalink }})  
    **Authors**: {{ .Params.authors }}  
    **Year**: {{ .Params.year }}  
{{ end }}