# Pain Package Registry

This is the official package registry for the [Pain programming language](https://github.com/pain-lng/pain).

## Structure

- `index/` - Hierarchical index for fast package lookup
- `packages/` - Package metadata files (TOML format)

## Publishing a Package

Use the `painpkg publish` command from your package directory:

```bash
cd your-package
painpkg publish
```

This will:
1. Create package metadata in `packages/{name}/{version}.toml`
2. Update the index in `index/...`
3. Create a branch and push changes
4. Provide a link to create a PR

## Installing Packages

```bash
painpkg add package-name
painpkg install
```

## Searching Packages

```bash
painpkg search query
```

## Documentation

See [docs/REGISTRY.md](../docs/REGISTRY.md) in the main Pain repository for detailed documentation.

## Contributing

To add a package to the registry:

1. Use `painpkg publish` from your package directory
2. Create a Pull Request with the generated changes
3. Wait for review and merge

## License

MIT License - see [LICENSE](LICENSE) file for details.

