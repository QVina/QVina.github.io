# Compiling QuickVina 2



1. **Please make sure you have _BOOST_ 1.60 at least installed**

1. Using git, clone the code:

      ```bash
      git clone https://github.com/QVina/qvina.git
      ```
 
1. Checkout the qvina 2 branch:

      ```bash
      cd qvina
      git checkout qvina2
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
    
      ```bash
      make
      ```

You will find an executable file called **qvina02** in the current folder.

