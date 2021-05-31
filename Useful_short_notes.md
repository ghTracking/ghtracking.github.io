# Useful short notes

### 21/03/21

Using RDkit to kekulize a molecule:

```python
#(https://sourceforge.net/p/rdkit/mailman/message/36893087/)

from rdkit import Chem
smi = "CN1C(NC2=NC=CC=C2)=CC=C1"
mol = Chem.MolFromSmiles(smi)

Chem.Kekulize(mol)
print(Chem.MolToSmiles(mol, kekuleSmiles=True))


```

RDkit and pandas seems to integrate well. https://www.youtube.com/watch?v=b5mz7cnA93A


To use RDkit with jupyter, run `conda install -n my-rdkit-env nb_conda_kernels` to ensure that the new environment can run jupyter.

