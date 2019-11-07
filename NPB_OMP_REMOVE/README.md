# cetus script

cetus_script.py is an script to run benchmark test of the NAS problems BT LU ...
it is ...

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

