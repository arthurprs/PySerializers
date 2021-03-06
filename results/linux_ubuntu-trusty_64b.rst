##############################
Python Serialization Benchmark
##############################

*               Platform : Linux-3.13.0-32-generic-x86_64-with-Ubuntu-14.04-trusty
*                 Python : CPython/2.7.6
*      Benchmark version : 1.2.0
*                 Run at : 2014-07-30 15:28:41.591691
*     Randomization seed : seed_thrift_vs_proto
* Benchmarks sample size : 128
*       Benchmark repeat : 128

NumStuff serialize
==================

* L1 : 4

+----------------------+----------+-----------+--------+
| framework            | status   | op_time   |   rank |
+======================+==========+===========+========+
| json 2.0.9           | OK       | 39.04 us  |   8.71 |
+----------------------+----------+-----------+--------+
| msgpack 0.4.2        | OK       | 4.48 us   |   1    |
+----------------------+----------+-----------+--------+
| protobuf/py 2.5.0    | OK       | 158.49 us |  35.35 |
+----------------------+----------+-----------+--------+
| thrift/py 0.9.0      | OK       | 71.80 us  |  16.02 |
+----------------------+----------+-----------+--------+
| protobuf/pyext 2.5.0 | OK       | 49.37 us  |  11.01 |
+----------------------+----------+-----------+--------+
| thrift/pyext 0.9.0   | OK       | 12.11 us  |   2.7  |
+----------------------+----------+-----------+--------+
| pycapnp 0.4.5        | OK       | 110.02 us |  24.54 |
+----------------------+----------+-----------+--------+

NumStuff deserialize
====================

* L1 : 4

+----------------------+----------+-----------+--------+
| framework            | status   | op_time   |   rank |
+======================+==========+===========+========+
| json 2.0.9           | OK       | 29.89 us  |   4.7  |
+----------------------+----------+-----------+--------+
| msgpack 0.4.2        | OK       | 6.36 us   |   1    |
+----------------------+----------+-----------+--------+
| protobuf/py 2.5.0    | OK       | 126.02 us |  19.82 |
+----------------------+----------+-----------+--------+
| thrift/py 0.9.0      | OK       | 108.40 us |  17.05 |
+----------------------+----------+-----------+--------+
| protobuf/pyext 2.5.0 | OK       | 58.19 us  |   9.15 |
+----------------------+----------+-----------+--------+
| thrift/pyext 0.9.0   | OK       | 16.29 us  |   2.56 |
+----------------------+----------+-----------+--------+
| pycapnp 0.4.5        | OK       | 59.29 us  |   9.33 |
+----------------------+----------+-----------+--------+

StringStuff serialize
=====================

* L1 : 4
* BS : 64

+----------------------+----------+-----------+--------+
| framework            | status   | op_time   |   rank |
+======================+==========+===========+========+
| json 2.0.9           | OK       | 28.79 us  |   3.11 |
+----------------------+----------+-----------+--------+
| msgpack 0.4.2        | OK       | 9.24 us   |   1    |
+----------------------+----------+-----------+--------+
| protobuf/py 2.5.0    | OK       | 88.03 us  |   9.52 |
+----------------------+----------+-----------+--------+
| thrift/py 0.9.0      | OK       | 70.80 us  |   7.66 |
+----------------------+----------+-----------+--------+
| protobuf/pyext 2.5.0 | OK       | 45.02 us  |   4.87 |
+----------------------+----------+-----------+--------+
| thrift/pyext 0.9.0   | OK       | 12.37 us  |   1.34 |
+----------------------+----------+-----------+--------+
| pycapnp 0.4.5        | OK       | 17.53 us  |   1.9  |
+----------------------+----------+-----------+--------+

StringStuff deserialize
=======================

* L1 : 4
* BS : 64

+----------------------+----------+-----------+--------+
| framework            | status   | op_time   |   rank |
+======================+==========+===========+========+
| json 2.0.9           | OK       | 116.47 us |  24.77 |
+----------------------+----------+-----------+--------+
| msgpack 0.4.2        | OK       | 4.70 us   |   1    |
+----------------------+----------+-----------+--------+
| protobuf/py 2.5.0    | OK       | 84.76 us  |  18.02 |
+----------------------+----------+-----------+--------+
| thrift/py 0.9.0      | OK       | 105.05 us |  22.34 |
+----------------------+----------+-----------+--------+
| protobuf/pyext 2.5.0 | OK       | 57.28 us  |  12.18 |
+----------------------+----------+-----------+--------+
| thrift/pyext 0.9.0   | OK       | 13.87 us  |   2.95 |
+----------------------+----------+-----------+--------+
| pycapnp 0.4.5        | OK       | 44.90 us  |   9.55 |
+----------------------+----------+-----------+--------+

ComboStuff serialize
====================

* L1 : 4
* BS : 64

+----------------------+----------+-----------+--------+
| framework            | status   | op_time   |   rank |
+======================+==========+===========+========+
| json 2.0.9           | OK       | 62.90 us  |   4.9  |
+----------------------+----------+-----------+--------+
| msgpack 0.4.2        | OK       | 12.85 us  |   1    |
+----------------------+----------+-----------+--------+
| protobuf/py 2.5.0    | OK       | 231.06 us |  17.99 |
+----------------------+----------+-----------+--------+
| thrift/py 0.9.0      | OK       | 136.15 us |  10.6  |
+----------------------+----------+-----------+--------+
| protobuf/pyext 2.5.0 | OK       | 86.10 us  |   6.7  |
+----------------------+----------+-----------+--------+
| thrift/pyext 0.9.0   | OK       | 16.08 us  |   1.25 |
+----------------------+----------+-----------+--------+
| pycapnp 0.4.5        | OK       | 126.66 us |   9.86 |
+----------------------+----------+-----------+--------+

ComboStuff deserialize
======================

* L1 : 4
* BS : 64

+----------------------+----------+-----------+--------+
| framework            | status   | op_time   |   rank |
+======================+==========+===========+========+
| json 2.0.9           | OK       | 145.68 us |  14.71 |
+----------------------+----------+-----------+--------+
| msgpack 0.4.2        | OK       | 9.90 us   |   1    |
+----------------------+----------+-----------+--------+
| protobuf/py 2.5.0    | OK       | 202.50 us |  20.44 |
+----------------------+----------+-----------+--------+
| thrift/py 0.9.0      | OK       | 203.96 us |  20.59 |
+----------------------+----------+-----------+--------+
| protobuf/pyext 2.5.0 | OK       | 106.05 us |  10.71 |
+----------------------+----------+-----------+--------+
| thrift/pyext 0.9.0   | OK       | 21.36 us  |   2.16 |
+----------------------+----------+-----------+--------+
| pycapnp 0.4.5        | OK       | 79.35 us  |   8.01 |
+----------------------+----------+-----------+--------+

ComboBunch serialize
====================

* L1 : 4
* BS : 64
* L2 : 32

+--------------------+----------+-----------+---------+
| framework          | status   | op_time   | rank    |
+====================+==========+===========+=========+
| json 2.0.9         | OK       | 5.30 ms   | 6.39    |
+--------------------+----------+-----------+---------+
| msgpack 0.4.2      | OK       | 1.07 ms   | 1.29    |
+--------------------+----------+-----------+---------+
| protobuf/py 2.5.0  | OK       | 31.35 ms  | 37.81   |
+--------------------+----------+-----------+---------+
| thrift/py 0.9.0    | OK       | 12.77 ms  | 15.40   |
+--------------------+----------+-----------+---------+
| protobuf/pyext     | CRASHED  | CRASHED   | CRASHED |
+--------------------+----------+-----------+---------+
| thrift/pyext 0.9.0 | OK       | 829.19 us | 1.00    |
+--------------------+----------+-----------+---------+
| pycapnp            | CRASHED  | CRASHED   | CRASHED |
+--------------------+----------+-----------+---------+

ComboBunch deserialize
======================

* L1 : 4
* BS : 64
* L2 : 32

+--------------------+----------+-----------+---------+
| framework          | status   | op_time   | rank    |
+====================+==========+===========+=========+
| json 2.0.9         | OK       | 13.78 ms  | 12.21   |
+--------------------+----------+-----------+---------+
| msgpack 0.4.2      | OK       | 1.13 ms   | 1.00    |
+--------------------+----------+-----------+---------+
| protobuf/py 2.5.0  | OK       | 22.28 ms  | 19.74   |
+--------------------+----------+-----------+---------+
| thrift/py 0.9.0    | OK       | 20.00 ms  | 17.72   |
+--------------------+----------+-----------+---------+
| protobuf/pyext     | CRASHED  | CRASHED   | CRASHED |
+--------------------+----------+-----------+---------+
| thrift/pyext 0.9.0 | OK       | 1.54 ms   | 1.36    |
+--------------------+----------+-----------+---------+
| pycapnp 0.4.5      | OK       | 4.69 ms   | 4.16    |
+--------------------+----------+-----------+---------+
