# Setting Up Pain Registry Repository

This directory contains template files for initializing the `pain-registry` repository.

## Initial Setup

1. **Clone the repository** (if not already done):
   ```bash
   git clone https://github.com/pain-lng/pain-registry.git
   cd pain-registry
   ```

2. **Copy template files**:
   ```bash
   # From the Pain repository root
   cp -r pain-registry-template/* pain-registry/
   # Or manually copy:
   # - README.md
   # - .gitignore
   # - index/.gitkeep
   # - packages/.gitkeep
   ```

3. **Commit initial structure**:
   ```bash
   git add .
   git commit -m "Initial registry structure"
   git push origin main
   ```

## Directory Structure

After setup, your repository should have:

```
pain-registry/
├── README.md
├── LICENSE
├── .gitignore
├── index/
│   └── .gitkeep
└── packages/
    └── .gitkeep
```

## Next Steps

Once the repository is set up, users can:

1. **Publish packages**:
   ```bash
   cd their-package
   painpkg publish
   ```

2. **Install packages**:
   ```bash
   painpkg add package-name
   painpkg install
   ```

3. **Search packages**:
   ```bash
   painpkg search query
   ```

## Maintenance

- Review and merge PRs from `painpkg publish`
- Ensure package metadata is valid
- Monitor for duplicate packages or version conflicts

