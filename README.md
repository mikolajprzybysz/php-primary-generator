# php-primary-generator

```
composer install
./vendor/bin/phpbench run PrimaryBench.php --report=all
```

```
+-----------------------------+------+------+----------+-------------+-------------+-------------+-------------+--------+---------+
| subject                     | revs | its  | mem      | best        | mean        | mode        | worst       | rstdev | diff    |
+-----------------------------+------+------+----------+-------------+-------------+-------------+-------------+--------+---------+
| benchPrimeNormal            | 200  | 1000 | 710,344b | 919.540μs   | 960.927μs   | 952.243μs   | 1,902.540μs | 5.03%  | 0.00%   |
| benchPrimeOldNormalWhile    | 200  | 1000 | 710,344b | 922.550μs   | 968.763μs   | 958.554μs   | 2,149.070μs | 5.54%  | +0.81%  |
| benchPrimeOldNormalFor      | 200  | 1000 | 710,344b | 943.865μs   | 1,009.332μs | 981.371μs   | 2,312.830μs | 8.18%  | +4.80%  |
| benchPrimeOldNormalGoto     | 200  | 1000 | 710,344b | 929.795μs   | 990.897μs   | 959.481μs   | 1,728.205μs | 8.92%  | +3.02%  |
| benchPrimeNormalWhileInline | 200  | 1000 | 710,344b | 933.705μs   | 1,005.046μs | 969.654μs   | 2,158.375μs | 11.05% | +4.39%  |
| benchPrimeGenerator         | 200  | 1000 | 833,088b | 1,055.245μs | 1,092.129μs | 1,083.591μs | 1,817.600μs | 3.90%  | +12.01% |
| benchPrimeGeneratorIf       | 200  | 1000 | 833,056b | 1,055.815μs | 1,095.657μs | 1,079.035μs | 1,903.340μs | 5.83%  | +12.30% |
| benchPrimeGeneratorGoto     | 200  | 1000 | 833,056b | 1,049.345μs | 1,082.866μs | 1,073.435μs | 1,733.245μs | 3.20%  | +11.26% |
+-----------------------------+------+------+----------+-------------+-------------+-------------+-------------+--------+---------+
```
