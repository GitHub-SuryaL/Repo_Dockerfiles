### ENTRYPOINT

ENTRYPOINT is also used to run the container just like CMD. But there are few differences.
1. We can't override ENTRYPOINT, but we can override CMD.  
2. We can't override ENTRYPOINT, if you try to do, it will go and append to the ENTRYPOINT command.
3. If you use both CMD & ENTRYPOINT in Dockerfile and don’t give any command from terminal (at runtime), CMD   acts as an argument provider to ENTRYPOINT
4. CMD will Supply default arguments to ENTRYPOINT
5. You can override CMD arguments from runtime 
6. We can stop misusing your image with other commands if you use ENTRYPOINT in Dockerfile 