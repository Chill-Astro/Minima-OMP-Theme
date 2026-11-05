<div align="center">  
    <img height="300" alt="Minama" src="https://github.com/user-attachments/assets/68699920-ad4c-4bcd-b662-b9e9a343a648" />
      
    
**Minima** is a *Simple but Universal Theme* for [Oh My Posh!](https://github.com/jandedobbeleer/oh-my-posh), Built for `Speed`, `Adaptability`, `Features` and `Maximum Portability`.

Made for ALL **Terminal Color Schemes**! In Demonstration, `Tokyo Night Storm` is Used.

**Latest Version** : `v1.1`

</div>

---

## Key Features :

- **NO NEED for Nerd Font**! ✅
- **Extremely Minimal and Fast!** ✅
- **Consistent on ALL SYSTEMS & Color Schemes!** ✅
- Handles **Root / Administrator** using `#` instead `$`! ✅
- **NO FEATURE CREEP!** Includes `Git Checks`, `Execution Time`, and `Highlighting $ / # to Red for Errors`. ✅
- **WORKS PERFECTLY** on ANY Garbage Terminal! ( Like `conhost.exe`) ! ✅

---

## Theme Code :

- Paste this Code in `~/AppData/Local/Programs/oh-my-posh/themes/Minima-PLUS.omp.json` if on Windows.
- Alternatively Paste it in  `~/.local/share/oh-my-posh/themes/Minima-PLUS.omp.json` if on Linux.
- You can Paste it Anywhere like `~/<randomfilepath>/Minima-PLUS.omp.json` on Windows, Linux or MacOS. ( Just Ensure that the Folder is Accessible )
- If on MacOS, GOOGLE IT!

      {
        "$schema": "https://raw.githubusercontent.com/JanDeDobbeleer/oh-my-posh/main/themes/schema.json",
        "blocks": [
          {
            "alignment": "left",
            "newline": false,
            "segments": [              
              {
                "foreground": "white",
                "style": "plain",
                "template": "{{ .UserName }}@{{ .HostName }} ",
                "type": "session"
              },
              {
                "foreground": "cyan",
                "options": {
                  "style": "full"
                },
                "style": "plain",
                "template": "{{ .Path }} ",
                "type": "path"
              },
              {
                "foreground": "blue",
                "style": "plain",
                "template": "› in {{ .FormattedMs }} ",
                "type": "executiontime"
              },
              {
                "foreground": "green",
                "options": {
                  "branch_icon": "› "
                },
                "template": "{{ .HEAD }} ",
                "style": "plain",
                "type": "git"
              },
              {
                "foreground": "white",
                "foreground_templates": [
                  "{{ if gt .Code 0 }}red{{ end }}"
                ],          
                "properties": {
                  "always_enabled": true
                },
                "style": "plain",
                "template": "{{ if .Root }}#{{ else }}${{ end }}",
                "type": "status"
              }
            ],
            "type": "prompt"
          }
        ],
        "final_space": true,
        "version": 4
      }
  
## Using this on Windows :

- Open Powershell Profile ( Replace `notepad` with `code`, `vim` or `nvim` if Preferred ) :

        notepad $Profile # or $Profile.AllUsersAllHosts
  
- Save this Text ( Change `pwsh` to `powershell` if using `Windows Powershell` ) :

Change the Path if Needed!

        oh-my-posh --init --shell pwsh --config ~/AppData/Local/Programs/oh-my-posh/themes/Minima-PLUS.omp.json | Invoke-Expression        

- Save this and Reload `Powershell Core` or `Windows Powershell`. Enjoy! :)

---

## Using this on Linux :

- Open your `.bashrc` ( Replace `nano` with `code`, `vim` or `nvim` if Preferred ) :

        nano ~/.bashrc
  
- Save this Text at the Bottom of File Contents ( Don't Overwrite ) :

Change the Path if Needed!

        eval "$(oh-my-posh init bash --config ~/.local/share/oh-my-posh/themes/Minima-PLUS.omp.json)"        

- Save this and Type :

        source ~/.bashrc
  
- Minima is Loaded. Enjoy! :)

---

## MacOS

¯\\\_(ツ)_/¯

---

## Credits :

- [Oh My Posh! by @jandedobbeleer](https://github.com/jandedobbeleer/oh-my-posh) : For Making Oh My Posh!
- [@Lisa on Pexels](https://www.pexels.com/photo/pink-flowers-photograph-1083822/) : For Wallpaper in Screenshots.
- [Windows Terminal by the Contributors @microsoft](https://github.com/microsoft/terminal) : Thanks for Replacing Conhost!

---

## Note from Developer :

A Star ⭐ will be Appreciated to Support this Project! :)

---   
