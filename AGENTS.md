---
published: false
---

# Interwoven Family Care Site Instructions

This repository is the website for Interwoven Family Care, a family care business run by Bri in Tacoma, Washington. The live site is a simple GitHub Pages-style static site for `interwoven.care`.

## People And Working Style

- Bri owns the business and is learning Git. She is smart, capable, determined, and new to this technical workflow.
- Drew is the technical helper and may coordinate setup, permissions, and repo mechanics.
- When working with Bri, use plain language, keep steps small, and explain what each Git or website action means.
- Treat Git as an empowering publishing ritual, not as a test. Avoid jargon unless Bri asks for it.
- Do not surprise-push. Only give publish steps or attempt publication after Bri says she is ready.

## Site Shape

- `index.html` is the live homepage.
- `CNAME` points GitHub Pages at `interwoven.care`.
- `assets/` contains logo, icon, and social preview images.
- The site is currently plain HTML/CSS/JS, with no build system.
- Keep changes simple and maintainable unless Drew or Bri asks for a larger redesign.

## Local Git Notes

In this Codex environment, Git may not be on `PATH`. The installed Git executable is:

```powershell
C:\Program Files\Git\cmd\git.exe
```

If Git reports dubious ownership for this repo, use this per-command flag:

```powershell
-c safe.directory='C:/IFC/interwoven.care'
```

Example read-only status command from Codex:

```powershell
& 'C:\Program Files\Git\cmd\git.exe' -c safe.directory='C:/IFC/interwoven.care' -C 'C:\IFC\interwoven.care' status --short --branch
```

Codex may have read access to this repo but not write access to `.git`, so staging and committing may need to happen in Bri's normal PowerShell window.

## Bri Commit Workflow

When Bri says she is ready to commit and publish, give her a small copy-paste loop for her normal PowerShell:

```powershell
cd C:\IFC\interwoven.care
git status
git add <changed-file>
git commit -m "Short description of the change"
git push
```

For multiple files:

```powershell
cd C:\IFC\interwoven.care
git status
git add index.html assets
git commit -m "Short description of the change"
git push
```

After she runs commands, help interpret Git output in everyday terms: what changed, whether it published, and what to do next.

## Safety And Care

- Before editing, inspect the current files and explain the intended change.
- Preserve Bri's voice and business positioning. Improve clarity without making the site feel generic.
- Keep accessibility, mobile layout, and contact links in mind.
- Use `bri@interwoven.care` as the current contact email unless Bri says otherwise.
- If adding a scheduler later, replace the booking mailto link deliberately and test it.
- If something goes wrong, stay calm and give recovery steps. The goal is confidence, not mystique.
