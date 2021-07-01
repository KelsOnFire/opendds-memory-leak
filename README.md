# opendds-memory-leak
Project to shared memory leak issue based on Messenger example

# How to build

1. Get Docker image with OpenDDS packages `docker pull kelsdev/ubuntu:latest`
2. Run docker image `docker run -it --network host -v $(pwd):/app kelsdev/ubuntu`
3. `mkdir /app/build && cd /app/build`
4. `cmake ..`
5. `make`

# How to run

`./publisher -DCPSConfigFile ../rtps.ini`

`./subscriber -DCPSConfigFile ../rtps.ini`
