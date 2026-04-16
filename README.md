# Shared Gaussian Splat Test Assets

Small, CC0-licensed Gaussian splat fixtures for integration tests, benchmarks, and format tooling across the 3DGS ecosystem.

## Files

| Asset | Files | Notes |
|--------|--------|--------|
| Cat figurine | `a_cute_cat_float32.spz` | Float32 splat data (SPZ) |
| Backpack | `adobe_backpack.ply`, `adobe_backpack.spz` | Same subject; Adobe-specific extensions in SPZ |
| Scarf | `scarf.ply`, `scarf.spz` | High quality; 4th-order SH in SPZ |
| Sparkling water | `sparkling_water.ply`, `sparkling_water.spz` | Reflective surface; visible 4th-order SH in SPZ |
| Seashell | `seashell.ply`, `seashell.spz` | A seashell with sophisticated texture |

**PLY** — Standard 3DGS point cloud; wide loader support. **SPZ** — Niantic’s compressed format; see [nianticlabs/spz](https://github.com/nianticlabs/spz).

## Usage

```bash
git clone https://github.com/raymondyfei/SharedTestModels.git
```

Point tests at local paths or fetch via raw URLs.

## License

[CC0 1.0 Universal](LICENSE) — use without restriction.
