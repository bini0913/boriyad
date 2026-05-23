# Binary Patch Report

Commit range: `HEAD^..HEAD`

Generated artifacts:
- `patches/pr-binary-safe.patch` (git format-patch --binary)
- `patches/pr-binary-safe.diff` (git diff --binary)

## Binary files changed

- `README.md`
  - sha256 before: `63e7cb389e0bb6f7773a1d3d977e224313bca162792d3dbb5f7102814336b146`
  - sha256 after: `9d3479227106960353a4bc2b76b6439c76af01222cef12a4604393d3323bb392`
  - binary patch file generated: included inside both artifacts above

## Apply instructions

Apply with git (preserves mode/metadata tracked by git):

```bash
git apply --index patches/pr-binary-safe.diff
# or
git am patches/pr-binary-safe.patch
```

Verify:

```bash
git status --short
git log --oneline -1
```
