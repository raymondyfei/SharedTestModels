# Shared Gaussian Splat Test Assets

A collection of Gaussian splat assets in various formats, intended as shared test fixtures for open-source software packages that work with 3D Gaussian splatting.

## Purpose

Consistent, freely available test assets make it easier to validate renderers, converters, viewers, and other tools across the Gaussian splat ecosystem. This repo provides a small set of real-world splats in multiple formats so projects can:

- Run integration and regression tests against known inputs
- Benchmark loading and rendering performance
- Test format conversion pipelines end-to-end

## Assets

| File | Format | Description |
|------|--------|-------------|
| `a_cute_cat_float32.ply` | PLY (float32) | A cat figurine, stored as a standard 3DGS PLY file with float32 attributes |
| `adobe_backpack.spz` | SPZ | A backpack, stored in the SPZ compressed splat format, containing Adobe-specific extensions |
| `scarf.spz` | SPZ | A high-quality scarf, stored in the SPZ compressed splat format, containing 4-th order spherical harmonics |
| `sparkling_water.spz` | SPZ | A shinny can of sparkling water, stored in the SPZ compressed splat format, containing visible 4-th order spherical harmonics |

## Formats

- **PLY** — The original 3D Gaussian Splatting point cloud format. Widely supported across loaders and viewers. Float32 variant stores per-Gaussian attributes (position, covariance, color/SH coefficients, opacity) as 32-bit floats.
- **SPZ** — A compressed binary format for Gaussian splats developed by Niantic. Significantly smaller file sizes than PLY. See [nianticlabs/spz](https://github.com/nianticlabs/spz) for the format spec and reference implementation.

## Usage

Clone the repo and point your tool or test suite at the files directly:

```bash
git clone https://github.com/raymondyfei/SharedTestModels.git
```

Or reference individual files via raw URL if your test infrastructure fetches remote assets.

## License

These assets are released under the [CC0 1.0 Universal](LICENSE) public domain dedication. You may use, modify, and distribute them for any purpose without restriction.
