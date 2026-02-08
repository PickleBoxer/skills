# Skills Repository

## Download Contents

Navigate to your target folder and run:

**Windows (PowerShell):**
```powershell
git clone https://github.com/PickleBoxer/skills.git temp_skills; Copy-Item -Path "temp_skills\*" -Destination "." -Recurse -Force; Remove-Item -Path "temp_skills" -Recurse -Force
```

**Linux/macOS:**
```bash
git clone https://github.com/PickleBoxer/skills.git temp_skills && cp -r temp_skills/* . && rm -rf temp_skills
```

This copies all repository contents to your current directory.
