# EPI, 1 month prep

### Hex to binary
0x1111 = 0b 1111 1111 1111 1111

### Extract first 4 bytes of a word
```
void ExtractBytes (uint32_t value) {
  uint32_t byte1 = value >> 24;
  uint32_t byte2 = (value >> 16) & 0xff;
  uint32_t byte3 = (value >> 8) & 0xff;
  uint32_t byte4 = value & 0xff;
  ...
}
```

### Count the # of 1 bits in an int
```
int CountBits (int x) {
  int num_bits = 0;
  while (x) {
    num_bits += x & 1;
    x >>= 1;
  }
  return num_bits;
}
```

### Set, clear, toggle bits
**Set** xth bit (0 being rightmost bit): ```number |= (1 << x);```  
0000 |= (1 << 3) => 0000 |= 1000 => 1000

**Clear** xth bit: ``` number &= ~(1 << x);```  
1111 &= ~(1 << 2) => 1111 &= ~(0100) => 1111 &= 1011 => 1011

**Toggle** xth bit, since 0^1=1 and 1^1=0: ``` number ^= (1 << x);```  
1111 ^= (1 << 1) => 1111 ^= 0010 => 1101  
0000 ^= (1 << 1) => 0000 ^= 0010 => 0010

- [ ] 5.3
- [ ] 5.11
- [ ] 6.5
- [ ] 6.8
- [ ] 7.7
- [ ] 7.8
- [ ] 8.10
- [ ] 9.3
- [ ] 9.9
- [ ] 10.11
- [ ] 11.5
- [ ] 12.5
- [ ] 12.10
- [ ] 13.4
- [ ] 13.7
- [ ] 14.6
- [ ] 14.9
- [ ] 15.5
- [ ] 15.9
- [ ] 16.4
- [ ] 16.9
- [ ] 17.5
- [ ] 17.7
- [ ] 18.8
- [ ] 19.3
- [ ] 20.9
- [ ] 21.1
