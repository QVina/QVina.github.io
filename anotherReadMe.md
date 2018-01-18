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
          
1. Build the application:
    
      ```bash
      make
      ```

You will find an executable file called **qvina-w** in the current folder.

