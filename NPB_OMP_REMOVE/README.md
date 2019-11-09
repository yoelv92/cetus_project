# cetus script

cetus_script.py is an script that the main purpose is to compile sourse to sourse using Cetus to make a parallel progrm and compile with icc Intel compiler or only compile with icc comlipler and run benchmark test of the NAS problems (BT,LU,MG,CG,EP,SP,UA), 
as a result before using the script must to load the Cetus compiler and Intel icc compiler.
the directives are:
```bash
module load intel

module load cetus
```
### Collaborative files
the files must be in the same directory with cetus_script.py.
run_
-dir 'path'	           	Path to the directory containing the tests   	default=current directory
-t <benchmark test>
    choos	test benchmark to run				default=run all the tests
-p			   	  compile the problem in parallel/serial     	default=not parallelize
-g			   	  send or not to grid     			default=not sending to grid
-c 'C/W' 		   	problem size 					default=problem size C


```bash
module load intel

module load cetus
```

##Usage
```bash
python3 cetus_test.py -dir <Path to the directory containing the tests> -t <test name to run> -p <turn on cetus complie> -g <send to the grid to run> 
```

