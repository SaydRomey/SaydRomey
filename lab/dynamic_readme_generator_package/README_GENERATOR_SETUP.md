# Dynamic README Generator Setup

Copy these files into your project root:

```text
readme.config.toml
README.template.md
tools/generate_readme.py
```

Generate the README:

```bash
python3 tools/generate_readme.py
```

Validate configured targets without writing:

```bash
python3 tools/generate_readme.py --check
```

Generate to a separate file for review:

```bash
python3 tools/generate_readme.py --output README.preview.md
```

When you move docs or assets, edit `readme.config.toml`, then regenerate.
