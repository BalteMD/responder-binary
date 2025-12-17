# Responder - Standalone Binary Builder


### Run the Binary

```bash
./Responder [options]
```

The binary is standalone and includes all dependencies

## Troubleshooting

### GLIBC Version Error

If you encounter an error like:
```
version `GLIBC_2.38' not found
```

This means your system's GLIBC is older than the one the binary was compiled with. The binary is built with Python latest image (typically GLIBC 2.31+), so your system needs at least that version.

**Solutions:**
1. **Check your GLIBC version**: `ldd --version`
2. **Use a compatible system**: The binary requires GLIBC 2.31 or higher