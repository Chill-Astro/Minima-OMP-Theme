<div align="center">  
    <img alt="Minama" width=700 src="https://github.com/user-attachments/assets/8beefe35-faa9-423f-b067-3af8d5c782bc" />
    
**Minima** is a *Simple but Universal Theme* for [Oh My Posh!](https://github.com/jandedobbeleer/oh-my-posh), Built for `Speed`, `Adaptability`, and `Maximum Portability`.

**Minima** is made for all sorts of Terminal Color Schemes. In the Preview, `Tokyo Night Storm` is Used.

Want an Advanced Edition? See [Minima PLUS!](https://github.com/Chill-Astro/Minima-PLUS-OMP)

Customization is Great, but not Inconvenience coming from Ricing. Thus I made a Simple Rice without any Dependencies. My Goal is to make Powershell look like Bash. Her Design is Inspired from the `Default Linux Terminal` and `adb shell` on Rooted Android.

**Latest Version** : `v1.3`

</div>

> [!NOTE]
> THIS THEME IS *"NOT FOR RICING LEGENDS"* NOR *"VERY ADVANCED USERS"*
> 
>( No Offence meant on Flexers and Ricing Legends. Sorry! :) )
---

## Key Features :

- No Need for Nerd Font. ✅
- Extremely Minimal and Fast. ✅
- Familiar from the Start, Consistent on ALL SYSTEMS. ✅
- Works on ANY Theme. ✅
- Handles Root Mode / Administrator Terminal using `$` or `#`, a Classic Linux-Style Convention. ✅
- COMES WITH NOTHING. ( Yes ) This doesn't have `Git Checks`, `Time`, `Newline` or `Fancy Iconography`. ✅
- Works Perfectly on Any Garbage Terminal, even `conhost.exe` that we know has Command Prompt. ✅
- Brings the Linux Terminal Style to `Windows Powershell` ( if using Windows! ) ✅

---

## Preview ( Sorry Arch Users this is Windows 11! ) :

<kbd>
<img alt="image" src="https://github.com/user-attachments/assets/a6b7bb4e-884d-4b3d-bfb5-9ce29bff6233" />
</kbd>

---

## Portability Showcase ( In conhost.exe ) :

Microsoft, if you are Seeing this, Please remove this from Home Systems, if not all. It's Terrible 🙏

<kbd>
<img alt="image" src="https://github.com/user-attachments/assets/36889c4d-3eff-4430-b7c7-975b387fa84c" />
</kbd>

---

## Theme Code :

- Paste this Code in `~/AppData/Local/Programs/oh-my-posh/themes/Minima.omp.json` if on Windows.
- Alternatively Paste it in  `~/.local/share/oh-my-posh/themes/Minima.omp.json` if on Linux.
- You can Paste it Anywhere like `~/<randomfilepath>/Minima.omp.json` on Windows, Linux or MacOS. ( Just Ensure that the Folder is Accessible )
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
                "foreground": "white",
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

        oh-my-posh --init --shell pwsh --config ~/AppData/Local/Programs/oh-my-posh/themes/Minima.omp.json | Invoke-Expression        

- Save this and Reload `Powershell Core` or `Windows Powershell`. Enjoy! :)

---

## Using this on Linux :

- Open your `.bashrc` ( Replace `nano` with `code`, `vim` or `nvim` if Preferred ) :

        nano ~/.bashrc
  
- Save this Text at the Bottom of File Contents ( Don't Overwrite ) :

Change the Path if Needed!

        eval "$(oh-my-posh init bash --config ~/.local/share/oh-my-posh/themes/Minima.omp.json)"        

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

## ⚠️ IMPORTANT NOTICE ⚠️

Please be aware: There are fraudulent repositories on GitHub that are cloning this project's name and using AI-generated readmes, but they contain **completely random and unrelated files in each release**. These are NOT official versions of this project.

**ALWAYS ensure you are downloading or cloning this project ONLY from its official and legitimate source:**
`https://github.com/Chill-Astro/Minima-OMP-Theme`

I am trying my best to report these people.

---

## ⚠️ Smoking Gun for Danger :

> [!CAUTION]
> **MALWARE ALERT:** If your downloaded folder looks like the images below, **DO NOT OPEN** any files. Format the drive or delete the folder immediately. Official releases are ONLY `.json` files.

<details>
<summary><b>View Details</b></summary>
  
* **Suspicious Windows Executables:** Files ending in `.exe`, `.bat`, or `.dll` (e.g., `luau.exe`, `StartApp.bat`).
* **Compressed Archives:** This project is distributed as a **JSON**, never as a `.zip` or `.7z` containing Windows binaries.
* **Hidden Scripts:** Text files like `asm.txt` used to execute malicious code on your PC.
* The Following Folder Structure is used by Malware (Shown in a VM) :

![Screenshot_2026-03-01-18-52-39-337_com clone android dual space](https://github.com/user-attachments/assets/be691c9f-7def-4e8b-982c-c7ca2e9a067d)

![Screenshot_2026-03-01-18-53-09-759_com clone android dual space](https://github.com/user-attachments/assets/1c75031d-95be-4716-9347-b762e3dad5b8)

</details>

---


## Note from Developer :

Appreciate my effort? Why not leave a Star ⭐ ! Also if forked, please credit me for my effort and thanks if you do! :)

---   
