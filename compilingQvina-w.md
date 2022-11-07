# Compiling QuickVina-W



1. **Please make sure you have _BOOST_ 1.60 at least installed**

1. Using git, clone the code:

      ```bash
      git clone https://github.com/QVina/qvina.git
      ```
 
1. Checkout the qvina-w branch:

      ```bash
      cd qvina
      git checkout qvina-w
      ```
     
1. If you installed boost in your home directory then edit the first two lines of Makefile:
   
      ```Makefile
      BASE = /Your/boost/location
      BOOST_VERSION=1_60 #or your installed version
      ```        
          
1. If you are using MacOS, edit the 4th line of the Makefile:
   
      ```Makefile
      C_PLATFORM=-static -pthread
      ```        
   to be
   
      ```Makefile
      C_PLATFORM= -pthread
      ```        

1. Build the application:
    
   In normal situations, it is enough to build QuickVina-W using the default configuration (parallel). just write:
   
      ```bash
      make
      ```
      You will find an executable file called **qvina-w** in the current folder.
      
    =================

    However, if you are running QuickVina-W on a single core, it would be more time efficient to build QuickVina-W for serial running. in such case you should write:
   
      ```bash
      make serial
      ```

    You will find an executable file called **qvina-w_serial** in the current folder.


