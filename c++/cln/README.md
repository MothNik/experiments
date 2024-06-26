Some examples of the use of the [CLN](https://www.ginac.de/CLN/).

* `exp_example.cpp`: exponentiate a high precision number.
* `asin_example.cpp`: compute the arcsine of a real number greater than 1.
* `log1p_example.cpp`: compute log1p(z) for a complex z.
* `doubledouble_log1p_ref.cpp`: compute log1p(z) for complex z, emulating the
  effect of creating z from a literal long double on a platform where long double
  is IBM double-double.
* `benktander2_cdf_demo.cpp`: CLN is used to compute the CDF of the
[Benktander type II probability distribution](https://en.wikipedia.org/wiki/Benktander_type_II_distribution).

  Compile the program with

  ```
  g++ benktander2_cdf_demo.cpp -o benktander2_cdf_demo -lcln
  ```
  
  The output of the program is
  
  ```
  x = 1.0000001L0
  a = 0.5L0
  b = 0.9999L0
  
  cdf(x, a, b) = 5.000999874874997092501056693626340584318213687587079246103609743580706239712768063525544815692096L-8
  ```
