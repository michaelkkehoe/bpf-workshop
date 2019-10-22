# Tutorials
## Helper Materials
* [BCC Python Developer Guide](https://github.com/iovisor/bcc/blob/master/docs/tutorial_bcc_python_developer.md)
* [BCC Reference Guide](https://github.com/iovisor/bcc/blob/master/docs/reference_guide.md)

## eBPF Tutorial tasks
### Excercise 1: Getting Started
1. Try the Python 'Hello World' (Lesson 1) example [here](https://github.com/iovisor/bcc/blob/master/docs/tutorial_bcc_python_developer.md#lesson-1-hello-world)
2. Try writing your own eBPF program with the 'sys_sync' (Lesson 2) example [here](https://github.com/iovisor/bcc/blob/master/docs/tutorial_bcc_python_developer.md#lesson-2-sys_sync)

### Excercise 2: Bitehost
1. Try the Python 'bitehist' (Lesson 9) example [here](https://github.com/iovisor/bcc/blob/master/docs/tutorial_bcc_python_developer.md#lesson-9-bitehistpy)
2. Now it's time to try writing your own tool, try the 'disklatency' (Lesson 10) tutorial [here](https://github.com/iovisor/bcc/blob/master/docs/tutorial_bcc_python_developer.md#lesson-10-disklatencypy)

### Excercise 3: Disksnoop
1. Try the Python 'disksnoop' (Lesson 6) example [here](https://github.com/iovisor/bcc/blob/master/docs/tutorial_bcc_python_developer.md#lesson-6-disksnooppy)
2. Now modify the program to print which Task/ PID is interacting with the disk

### Excercise 4: TCPConnect
1. Try running the [tcpv4connect.py](https://github.com/iovisor/bcc/blob/master/examples/tracing/tcpv4connect.py) script in the [tracing folder](https://github.com/iovisor/bcc/tree/master/examples/tracing)
2. Make a copy of this program and add functionality to print when a TCP connection is closed (Hint: You can find the available tracing funtions in `/sys/kernel/debug/tracing/available_filter_functions`)

### Excercise 5: DDOS 
1. Write a program to detect a DDOS (More than 1000 packets in 1000000ns) coming to port TCP/80 from the "localhost" source-address by attaching a program to a raw socket (`attach_raw_socket()`)
> Hints:
* Use the `mtr` program to test your code: `sudo yum install mtr`
* Look at the [dns_matching.py](https://github.com/iovisor/bcc/blob/master/examples/networking/dns_matching/dns_matching.py) and [dddos.py](https://github.com/iovisor/bcc/blob/master/examples/tracing/dddos.py) files

### Extra Study
* You can find extra tutorials from Sasha Goldstein [here](https://github.com/goldshtn/linux-tracing-workshop)
* You can find extra examples in the Linux Kernel (written in C) [here](https://github.com/torvalds/linux/tree/master/samples/bpf)
