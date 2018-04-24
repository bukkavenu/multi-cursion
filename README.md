# multi-cursion
Multi-cursion is simply obtaining the loop feature using only functions without formally using 'for' or 'while' or 'do-while' or enumerators 

# Example:
    
    void a()
    {
      //return; -------------------------(1)
      b();
    }
    void b()
    {
      //return; -------------------------(2)
      c();
    }
    void c()
    {
      //return; --------------------------(3)
      a();
    }

## Here you can see function a() is calling b(); function b() is calling c() and function c() is calling a() which will indefinitely be in infinite loop unless there's a return statement at the beginning of either a() or b() or c()
   
    a() -> b() -> c() -> a() 
    /* which will be infinite loop unless the controls exits from either a() or b() or c()
    without executing the other function calls */


## Note: 
(i)We can use 2 or more functions to obtain the feature 

(ii)Just one return statement at either of the points (1) or (2) or (3) exits the loop
