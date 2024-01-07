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

kema

    // {
    //   "type": "argocd",
    //   "tips": ["argo", "argocd"],
    //   "style": "diamond",
    //   "leading_diamond": "",
    //   "trailing_diamond": " ",
    //   "foreground": "#ef754f",
    //   "background": "background",
    //   "template": "󱣘 {{ if .User }}{{ .User }}{{ end }}{{ if .Server }}{{ if .User }}@{{ end }}{{ .Server }}{{ end }}{{ if .Name }}{{ id or .User .Server }} :: {{ end }}{{ .Name }}{{ end }}"
    // },

            // {
        //   "type": "elixir",
        //   "style": "diamond",
        //   "leading_diamond": "",
        //   "trailing_diamond": " ",
        //   "foreground": "#4e2a8e",
        //   "background": "background",
        //   "properties": {
        //     "home_enabled": false,
        //     "fetch_version": true,
        //     "display_mode": "files"
        //   },
        //   "template": " {{ if .Full }}{{ .Full }}{{ end }}"
        // },

<parentBackground>\ue0b0</>


unknownPoshTheme
        {
          "type": "battery",
          "style": "powerline",
          "powerline_symbol": "\ue0b6",
          "invert_powerline": true,
          "foreground": "p:text",
          "background_templates": [
            "{{if and ( lt .Percentage 10 ) (eq \"Charging\" .State.String)}}p:battery_low{{end}}",
            "{{if and ( lt .Percentage 10 ) (eq \"Discharging\" .State.String)}}p:battery_critical{{end}}",
            "{{if lt .Percentage 50 }p:battery_halfway{{end}}",
            "p:battery_halfway"
          ],
          "template": " {{ if and ( not .Error) ( lt .Percentage 50 )  }}{{ .Icon }}{{ .Percentage }}%{{ end }} ",
          "properties": {
            "charged_icon": "\udb80\udc79 ",
            "charging_icon": "\udb80\udc84 ",
            "discharging_icon": "\udb80\udc8c "
          }
        },