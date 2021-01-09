# Port-Scanner
Using C++ language to scan all the available open/closed network ports on a device using IP address of the host and no other additional resources used.

#Commands

  To compile the Port Scanner Program
  
          → gcc port_scanner_code.cpp -o port_scanner
             * Here port_scanner_code.cpp is the source code which is                    
                compiled using gcc and the output/executable file is port_scanner.
                
  To run the code 
  
        → ./port_scanner 127.0.0.1 21 443
           * Here ./port_scanner runs the code in the command line, 127.0.0.1 is the IP we
              want to do  the scan on, 21 is the starting Port and 443 is the last one.



#Port Demonstration 

  Since we are testing on a local machine, there were no ports open at the time. 
So we started a server at port 80 using this command:

  → service apache2 start
 
Now the port 80 is open and a server is running on this machine.
Now to check whether this port is open or not we run our port scanner to check the available ports.

   → ./port_scanner 127.0.0.1 75 82
 
It is visible that the port 80 is open and all  other ports are closed.
