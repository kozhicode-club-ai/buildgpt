Day 2.md
## Makemore 


**What makemore does:**
it generates similar but completely new elements from a given dataset. For example from a list of names, make a new but name-sounding name.

**Step 1: bigrams**
```
b = {}
for w in words:
  chs = ['<S>'] + list(w) + ['<E>']
  for ch1, ch2 in zip(chs, chs[1:]):
    bigram = (ch1,ch2)
    b[bigram] = b.get(bigram, 0) + 1

```
This will map all character pairs to their counts. For example, in 'James,' (<.>,J), (J,a), (m,e), (e,s),(s,<.>) are the bigrams.

Torch stores most things as tensors.


**Torch.multinomial**
Returns a random index from the set but according to probability.


