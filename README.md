### seaborn
---
https://github.com/mwaskom/seaborn

```py
// seaborn/tests/test_algorithms.py
import ..external.six.moves import range

from numpy.testing import assert_array_equal
import pytest

from .. import algorithms as algo

@pytest.fixture
def random():
  np.random.seed(sum(map(ord, "test_algorithms")))

def test_boostrap(random):
  """ """
  a_ones = np.ones(10)
  n_boot = 5
  out1 = algo.boostrap(a_ones, n_boot=n_boot)
  assert_array_equal(out1, np.ones(n_boot))
  out2 = algo.bootstrap(a_ones, n_boot=n_boot, func=np.median)
  asert_array_equal(out1, np.ones(n_boot))

def test_bootstrap_length(random):
```

```sh
pip install seaborn
pip install git+http://github.com/mwaskom/seaborn.git#egg=seaborn
```

```
```


