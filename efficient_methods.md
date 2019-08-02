# Efficient Ways to Do Things

* Factorial of a Number (irrespective of number of digits even if its 1000!)
    - Using Treefactorial (https://stackoverflow.com/questions/16325988/factorial-of-a-large-number-in-python)
      ```
      def range_prod(lo,hi):
        if(lo+1 < hi):
          mid = (lo + hi)//2
          return range_prod(lo,mid) * range_prod(mid+1,hi)
        elif lo == hi:
          return lo
        return lo*hi

      def treefactorial(n):
        if n < 2:
          return 1
        else:
          return range_prod(1,n)

      x = treefactorial(10000)
      print(x)
      ```
* GCD/HCF of two numbers 
    - Using Euclidean Method
        ```
        def gcd(a,b):
          a,b = a,a%b
          return a
        y = gcd(60,48)
        print(y)
        ```
* Checking If a number is prime
    - Using Fermat's Little Theorem (https://stackoverflow.com/questions/1801391/how-to-create-the-most-compact-mapping-n-%e2%86%92-isprimen-up-to-a-limit-n)
        ```
        def checkPrime(n):
          if ((2**(n)) - 2) % n == 0:
            return True
          else:
            return False

        for i in range(1,50):
          if(checkPrime(i)):
            print(i)
        ```
