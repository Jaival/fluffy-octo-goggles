- 
  \uf74a - most probably it is space

  "tooltips": [
  {
  "type": "git",
  "tips": ["git", "g"],
  "style": "diamond",
  "foreground": "#193549",
  "background": "#fffb38",
  "leading_diamond": "",
  "trailing_diamond": "",
  "template": "{{ .HEAD }}{{ if .Staging.Changed }}  {{ .Staging.String }}{{ end }}{{ if and (.Working.Changed) (.Staging.Changed) }} |{{ end }}{{ if .Working.Changed }}  {{ .Working.String }}{{ end }}",
  "properties": {
  "fetch_status": true,
  "fetch_upstream_icon": true
  }
  }
  ],
  {{ .Segments.Time.CurrentDate | date \"15:04:05\" }}