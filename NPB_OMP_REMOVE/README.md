# cetus script

cetus_script.py is an script that the main purpose is to compile sourse to sourse using Cetus to make a parallel progrm and compile with icc Intel compiler or only compile with icc comlipler and run benchmark test of the NAS problems (BT,LU,MG,CG,EP,SP,UA), 
as a result before using the script must to load the Cetus compiler and Intel icc compiler.
the directives are:
```sh
$ module load intel

$ module load cetus
```
### Collaborative files:
#### The files must be in the same directory with cetus_script.py.
* [Makefile](https://github.com/yoelv92/cetus_project/blob/master/NPB_OMP_REMOVE/Makefile) - Use to compile the tests
* [run_test.py](https://github.com/yoelv92/cetus_project/blob/master/NPB_OMP_REMOVE/run_tests.py) - The script ment for runig the tests after compiling . 
### Script options: 
| Option | Description | Default |
| ------ | ------ | ------ |
| -dir | Path to the directory containing the benchmark tests directorys | Current directory |
| -c | The size for the input class C or W  | C |
| -t | Choosing which benchmark test to run (BT,LU,MG,CG,EP,SP,UA)  | Run all |
| -p | Compile sourse to sourse using Cetus to make benchmark test run in parallel | Not parallelize the benchmark test |
| -g | Sending the benchmark test to run in the grid  | Not sending to grid |

#### To execute:
```sh
$ python3 cetus_test.py  -dir <path> -c <class> -t <test> 
```

