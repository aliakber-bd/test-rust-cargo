# Test Rust Project (CARGO)

Tests component locator support for CARGO package manager.

## Vulnerable Dependencies
- `serde 1.0.100` - Old version
- `regex 1.3.0` - Old version with potential issues
- `openssl 0.10.25` - Known vulnerabilities
- `tokio 0.2.0` - Old version

## Expected Behavior
When Blackduck Detect runs:
1. Detects CARGO package manager
2. Finds vulnerable components in Cargo.toml
3. Component locator should process (not skip) CARGO manager
4. Locates components in Cargo.toml file
