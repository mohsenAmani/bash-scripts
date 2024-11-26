### README.md

```markdown
# Stress Test Script

A simple script to perform stress tests on system resources like CPU, memory, and storage.
It allows you to evaluate the performance and stability of your system under heavy load conditions.

---

## How to use:

```bash
Usage: stress-test.sh [OPTIONS]
Options:
    -h, --help      Show this help output
    -t, --timeout   Duration for the test (e.g., 60s, 5m, 1h). Default: Runs indefinitely.
```

---

## Prerequisites:

Ensure the following tools are installed on your system:

1. **`stress-ng`** - Used for CPU and memory stress tests.
   - Install via `apt`: 
     ```bash
     sudo apt install stress-ng
     ```
   - [Official Documentation](https://wiki.ubuntu.com/Kernel/Reference/stress-ng)

2. **`fio`** - Used for storage stress tests.
   - Install via `apt`: 
     ```bash
     sudo apt install fio
     ```
   - [Official Documentation](https://fio.readthedocs.io/)

---

## Example:

```bash
# Run a memory stress test for 5 minutes
./stress-test.sh -t 5m

# Run a CPU stress test indefinitely
./stress-test.sh

# Run the script with help output
./stress-test.sh -h
```

---

## Notes:

- The script will prompt for confirmation before running any test to avoid accidental execution.
- Ensure this is not run in a production environment to prevent system unresponsiveness.
- Use responsibly and monitor system behavior during stress testing.

---

## License

This script is open-source and distributed under the MIT License. See the `LICENSE` file for more details.
```

---
