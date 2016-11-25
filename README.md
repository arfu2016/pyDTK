# dtk

python implementation of distributed tree kernel.

# Installation
```
cd <folder> 
pip3 install .
```
# Usage
```
from pydtk.tree import Tree
from pydtk.dtk import DT
from pydtk.operation import fast_shuffled_convolution

tree = Tree(string="(A (B C)")
dtCalculator = DT(dimension=8192, LAMBDA= 0.6, operation=fast_shuffled_convolution)

distributedTree = dtCalculator.dt(tree)

>> array([-0.00952759,  0.02018453, -0.02713741, ...,  0.00362533,
       -0.02406953,  0.01796858])
       
```


