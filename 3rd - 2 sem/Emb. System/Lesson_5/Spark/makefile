CC=g++
CFLAGS=-g -c -Wall

all: SFE_LSM9DS0.o SparkFun_9DOF_main.o
	$(CC) -o EdisonV3 SFE_LSM9DS0.o SparkFun_9DOF_main.o -lmraa

SFE_LSM9DS0.o: SFE_LSM9DS0.cpp SFE_LSM9DS0.h
	$(CC) $(CFLAGS) SFE_LSM9DS0.cpp -lmraa

SparkFun_9DOF_main.o: SparkFun_9DOF_main.cpp SFE_LSM9DS0.h
	$(CC) $(CFLAGS) SparkFun_9DOF_main.cpp -lmraa

clean:
	rm -rf *.o EdisonV3