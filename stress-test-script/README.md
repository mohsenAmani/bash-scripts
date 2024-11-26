# Stress Test Script

A simple script to perform stress tests on system resources like CPU, memory, and storage. It allows you to evaluate the performance and stability of your system under heavy load conditions.

## Usage

```bash
stress [OPTIONS]

Options:
  -h, --help      Show this help output
  -t, --timeout   Duration for the test (e.g., 60s, 5m, 1h). Default: Runs indefinitely.
```

## Prerequisites

The following tools must be installed on your system:

### stress-ng
Used for CPU and memory stress tests.

Install via apt:
```bash
sudo apt install stress-ng
```

For more information, see the [Official Documentation](https://wiki.ubuntu.com/Kernel/Reference/stress-ng)

### fio
Used for storage stress tests.

Install via apt:
```bash
sudo apt install fio
```

For more information, see the [Official Documentation](https://fio.readthedocs.io/)

## Examples

Run a memory stress test for 5 minutes:
```bash
./stress -t 5m
```

Run a CPU stress test indefinitely:
```bash
./stress
```

Show help output:
```bash
./stress -h
```

## Important Notes

- The script will prompt for confirmation before running any test to avoid accidental execution
- Do not run this in a production environment to prevent system unresponsiveness
- Use responsibly and monitor system behavior during stress testing

## License

This project is open source and available under the MIT License.
