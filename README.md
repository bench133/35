# 35
code9
from math import *
for i in range(32):
    ip = (129 << 24) | (0 << 16) | (2 << 8) | (176 << 0)
    mask = (2**i - 1) << (32 - i)
    if  f'{ip & mask:b}'.count('1') == f'{ip & (2**(32 - i) - 1):b}'.count('1'):
        print(comb(32 - i, f'{ip & mask:b}'.count('1')))
 
