# cetus script

cetus_script.py is an script that the main purpose is to compile sourse to sourse using Cetus to make a parallel progrm and compile with icc Intel compiler or only compile with icc comlipler and run benchmark test of the NAS problems (BT,LU,MG,CG,EP,SP,UA), 
as a result before using the script must to load the Cetus compiler and Intel icc compiler.
the directives are:
```sh
module load intel

module load cetus
```
### Collaborative files:
#### The files must be in the same directory with cetus_script.py.
* run_test.py
* Makefile

### Script options:
* -dit <path> -Path to the directory containing the benchmark tests directorys (default=current directory)
 
| Option | Description |Default|
| ------ | ------ | ------ |
| -dir | Path to the directory containing the benchmark tests directorys | Current directory |
| -c | The size for the input C or W  | C |
| -t| Choosing which benchmark test to run (BT,LU,MG,CG,EP,SP,UA)  | Run all |
| -p | Compile sourse to sourse using Cetus to make benchmark test run in parallel | not parallelize the benchmark test |
| -g | Sending the benchmark test to run in the grid  | not sending to grid |


##Usage
```bash
python3 cetus_test.py -dir <Path to the directory containing the tests> -t <test name to run> -p <turn on cetus complie> -g <send to the grid to run> 
```

