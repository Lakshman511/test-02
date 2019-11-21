# test-02
## Result
ACCURACY - 99.45%
PARAMETERS - 15K(15548)

## Strategy
convolution block1
28x28x1 | (3x3x1)x16 | 26x26x16
batch normalization
dropout(8%)
convolution block2
26x26x16 | (3x3x16)x32 | 24x24x32
batch normalization
dropout(8%)
convolution block3
24x24x1 | (3x3x16)x10 | 24x24x10
batch normalization
dropout(8%)
Maxpooling(2x2)
convolution block4
12x12x10 | (3x3x10)x16 | 10x10x16
batch normalization
dropout(8%)
convolution block5
10x10x1 | (3x3x16)x16 | 8x8x16
batch normalization
dropout(8%)
convolution block6
8x8x1 | (3x3x16)x16 | 6x6x16
batch normalization
dropout(8%)
convolution block6
6x6x1 | (3x3x16)x16 | 4x4x16
batch normalization
dropout(8%)
convolution block7
4x4xx1 | (3x3x10)x16 | 2x2x10
batch normalization
dropout(8%)
convolution block8
2x2x10 | (2x2x10)x10 | 1x1x10
here we flattened......
and normalized...
But here we didn't removed dropouts because it is the final data
