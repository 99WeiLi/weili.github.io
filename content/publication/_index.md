---
1. title: Publications
cms_exclude: true

# View.
view: citation

# Optional header image (relative to `static/media/` folder).
banner:
  caption: ''
  image: ''

{{ $counter := 1 }}  <!-- Initialize a counter variable -->
{{ range .Pages }}
  - **{{ $counter }}.** [{{ .Title }}]({{ .Permalink }})  
    **Authors**: {{ .Params.authors }}  
    **Year**: {{ .Params.year }}  
  {{ $counter = add $counter 1 }} <!-- Increment the counter for the next publication -->
{{ end }}
---
