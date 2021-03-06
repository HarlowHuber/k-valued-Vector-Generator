# k-valued--Vector--Generator
This program generates all possible k-valued vectors for a given vector of k-values, where k = (k1, k2, k3, kn, kn+1, ...). Each vector can be defined by its mixed-base value. A mixed-base value is similar to a decimal value, but each value of the vector that the value is calculated from could have a different base. If k = 2 for each vector attribute, then the mixed-base value is simply the decimal value. If k = (k1, k2, k3) for a vector x = (x1, x2, x3), then the mixed-base value would be calculated by:<br /> x1 * k1^2 + x2 * k2^1 + x3 * k3^0. 

For a vector of (1, 1, 1) and k = (3, 2, 5), then the mixed-base value will be 12. Using the previous vector, if k = (2, 2, 2), then the mixed-base value would be 7, essentially the decimal value since each k-value is 2 (the vector is a binary number).

The number of vectors generated can be calculated by multipling each k-value against each other. 
For example, if k = (2, 2, 2), there will be 8 binary vectors generated, ordered by there Hamming norm (the sum of the vectors), and sorted by the mixed-base value of the vector: 

   Hamming norm = 3<br />
   1, 1, 1

   Hamming norm = 2<br />
   1, 1, 0<br />1, 0, 1<br />0, 1, 1

   Hamming norm = 1<br />
   1, 0, 0<br />0, 1, 0<br />0, 0, 1

   Hamming norm = 0<br />
   0, 0, 0
