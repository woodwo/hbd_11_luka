# hbd_11_luka

```
samples({
  p: ['samples/sample_001.wav', 'samples/sample_020.wav', 'samples/sample_022.wav'],
  t: ['samples/sample_002.wav', 'samples/sample_025.wav', 'samples/sample_030.wav'],
  k: ['samples/sample_003.wav', 'samples/sample_015.wav', 'samples/sample_035.wav'],
  b: ['samples/sample_005.wav', 'samples/sample_010.wav', 'samples/sample_040.wav'],
  f: ['samples/sample_050.wav', 'samples/sample_055.wav', 'samples/sample_060.wav'],
  s: ['samples/sample_065.wav', 'samples/sample_070.wav', 'samples/sample_075.wav'],
  m: ['samples/sample_110.wav', 'samples/sample_115.wav', 'samples/sample_120.wav'],
  ah: ['samples/sample_170.wav', 'samples/sample_175.wav', 'samples/sample_180.wav'],
  boom: ['samples/sample_215.wav', 'samples/sample_220.wav', 'samples/sample_225.wav'],
  fx1: 'samples/sample_245.wav',
  fx2: 'samples/sample_250.wav'
}, 'https://raw.githubusercontent.com/woodwo/hbd_11_luka/main/');

stack(
    s("p t k b, m ah").slow(1.5),
    // Percussion
    s("t k").euclid(5, 32).slow(4),
)._punchcard()
```