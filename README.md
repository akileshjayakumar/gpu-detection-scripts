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
- No required environment variables are documented for basic usage.

## Usage
```bash
python gpu_test.py
```

## Contributing and Testing
- Contributions are welcome through pull requests with clear, scoped changes.
- Run the following checks before submitting changes:
```bash
python -m pytest
```

## License
Licensed under the `MIT` license. See [LICENSE](./LICENSE) for full text.
