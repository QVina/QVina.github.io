# Compiling QuickVina-W



1. *Please make sure you have _BOOST_ 1.60 at least installed*

1. Using git, clone the code:

      `git clone https://github.com/QVina/qvina.git`   
 
1. Checkout the qvina-w branch:

      `cd qvina`  
      `git checkout qvina-w`
     
1. If you installed boost in your home directory then edit the first line of Makefile:
   
      `BASE=/Your/boost/location`
      
    
1. Build the application:
    
      `make`

You will find an executable file called qvina-w in the current folder.

