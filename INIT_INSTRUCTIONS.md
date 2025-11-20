# Instructions for Initializing pain-registry Repository

## What to Do

1. **Go to your pain-registry repository**:
   ```bash
   cd path/to/pain-registry
   # Or clone it:
   git clone https://github.com/pain-lng/pain-registry.git
   cd pain-registry
   ```

2. **Copy these files to the repository root**:
   - `README.md` → root of pain-registry
   - `.gitignore` → root of pain-registry

3. **Create directory structure**:
   ```bash
   mkdir -p index packages
   touch index/.gitkeep packages/.gitkeep
   ```

4. **Commit and push**:
   ```bash
   git add .
   git commit -m "Initial registry structure"
   git push origin main
   ```

## Files to Copy

From `pain-registry-template/` directory:
- ✅ `README.md` - Main repository README
- ✅ `.gitignore` - Git ignore rules
- ✅ `index/.gitkeep` - Keep index directory in git
- ✅ `packages/.gitkeep` - Keep packages directory in git

## Verification

After setup, test that it works:

```bash
# From any Pain project
painpkg search test
```

This should work without errors (even if no packages are found yet).

## Done!

Once initialized, the registry is ready for:
- Publishing packages (`painpkg publish`)
- Installing packages (`painpkg install`)
- Searching packages (`painpkg search`)

