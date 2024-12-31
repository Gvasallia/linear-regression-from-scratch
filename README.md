# Linear Regression from Scratch

This project implements Linear Regression from scratch using NumPy. It includes a complete implementation with gradient descent optimization, example usage, and comprehensive tests.

## Features

- Implementation of Linear Regression using gradient descent
- Support for multiple features
- R² score calculation
- Comprehensive test suite
- Example usage

## Installation

```bash
pip install -r requirements.txt
```

## Usage

```python
from linear_regression.model import LinearRegression
import numpy as np

# Generate sample data
X = 2 * np.random.rand(100, 1)
y = 4 + 3 * X + np.random.randn(100, 1)

# Create and train model
model = LinearRegression(learning_rate=0.01, n_iterations=1000)
model.fit(X, y.ravel())

# Make predictions
y_pred = model.predict(X)

# Calculate R² score
score = model.score(X, y.ravel())
```

## Testing

Run tests using pytest:

```bash
pytest tests/
```

## License

MIT

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.