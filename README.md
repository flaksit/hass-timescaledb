# Home Assistant TimescaleDB Add-on

[![License](https://img.shields.io/github/license/flaksit/hass-timescaledb-addon)](LICENSE)

A Home Assistant add-on providing PostgreSQL 18 with [TimescaleDB](https://www.timescale.com/) 2.25 — a high-performance time-series database optimized for the Raspberry Pi 5.

## Features

- PostgreSQL 18 with TimescaleDB 2.25 extension pre-loaded
- Optimized defaults for Raspberry Pi 5 (4GB/8GB)
- Configurable tuning via the add-on UI (shared_buffers, work_mem, etc.)
- Proper process management with s6-overlay (graceful shutdown, signal handling)
- Health monitoring via pg_isready watchdog

## Getting Started

1. Add this repository to your Home Assistant add-on store:

   `https://github.com/flaksit/hass-timescaledb-addon`

2. Install the "TimescaleDB" add-on
3. Start the add-on

See the [full documentation](timescaledb/DOCS.md) for configuration options.

## Architecture

| Component | Version |
|-----------|---------|
| PostgreSQL | 18 |
| TimescaleDB | 2.25.2 |
| s6-overlay | 3.2.2.0 |
| Target | aarch64 (Raspberry Pi 5) |

## License

See [LICENSE](LICENSE).
