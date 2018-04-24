# multi-cursion
Multi-cursion is simply obtaining the loop feature using only functions without formally using 'for' or 'while' or 'do-while' or enumerators 

# Example:
    
    void a()
    {
      b();
    }
    void b()
    {
      c();
    }
    void c()
    {
      a();
    }

## Here you can see function a() is calling b(); function b() is calling c() and function c() is calling a() which will indefinitely be in infinite loop unless there's a return statement at the beginning of either a() or b() or c()
   
    a() -> b() -> c() -> a() 
    /* which will be infinite loop unless the controls exits from either a() or b() or c()
    without executing the other function calls */
