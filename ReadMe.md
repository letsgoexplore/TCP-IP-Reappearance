## About the Project

### What is This Project?

This is the experiment of Computer Networking, provided by Department of Automation, Tsinghua University. Credited to https://gitee.com/Starrah/tcp-impl.git.

### What funtion does it realize?

This project reappears the TCP/IP protocal. It's capable of establishing connection, transferring messages and destroying connection. Retransmission timeout to be added.

### What's its core logic?

The core of TCP/IP is FSM(Finite State Machine). Our essential mission is to reappear the transition of the FSM. The movement of the FSM can be viewed in `FSM.png` in the first-level directory.

### What about its project structure?

In this project, we mainly focus on the Transmission Layer. Other layers like Application layer and Network layer will be simulated through the `driver` in the second-level directory, and the <api> in the third-level directory. 

## How to run the code?

### Environment

Ubuntu=22.4
wireshark : An app to catch the transmitting package.

```
sudo apt install git curl python3-pip wireshark
sudo usermod -aG wireshark $USER
```

### Run the code

open a new terminal at the same directory of the `driver`, and type:

```
sudo ./driver
```

Then the server is on.
After this open another terminal at the directory of the `main.py`

```
python main.py
```