# GPU Detection Scripts
Small Python utilities to quickly verify whether your machine can see GPUs through PyTorch and TensorFlow.

## Quick Start
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python gpu_test.py
```

## Capabilities
- Check CUDA visibility and device details via PyTorch (`gpu_test_pytorch.py`).
- Check visible GPU count via TensorFlow (`gpu_test_tf.py`).
- Run a combined check in one command (`gpu_test.py`).
- Gracefully report missing frameworks instead of crashing.

## Configuration
- No required environment variables.
- Optional: activate the correct environment for your CUDA drivers/toolkit before running checks.

## Usage
Run all checks:
```bash
python gpu_test.py
```

Run only the PyTorch check:
```bash
python gpu_test_pytorch.py
```

Run only the TensorFlow check:
```bash
python gpu_test_tf.py
```

## Contributing and Testing
- Open an issue or PR with improvements to script output or compatibility.
- Run tests with:
```bash
pytest
```
- Tests execute each script end-to-end from `tests/test_scripts.py`.

## License
Licensed under the `MIT` license. See [LICENSE](./LICENSE) for full text.
