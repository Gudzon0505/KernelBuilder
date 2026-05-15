P2P v8C.2 Master Assembly Document. Three build sizes:
- MINIMAL (~80K tokens): preloader + core + essential live components
- STANDARD (~150K tokens): recommended for most production deployments — core, db, agents
- FULL (~300K tokens): includes debugging, exploration, memory, vendor tiers

Assembly rules: _preloader.md loads first; XML tags cannot be fragmented across file boundaries; YAML frontmatter removable in API deployments. Bash script example for concatenation. Python code for Anthropic prompt caching (70–90% cost reduction, 1024-token minimum).
