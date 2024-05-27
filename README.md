# Arrays and Methods

## Arrays as parameters
When passing an array as a parameter to a method, you are passing a reference to the array, therefore, the parameter variable in the method points to the same array as the calling program.

In the image below, the `sumArray` method computes the sum of the given array.  Notice that when executing `sumArray`, the parameter variable myArray points to the same array as the intArray variable.

```
public class Problem1 extends ConsoleProgram {
    public void run() {
    
    int[] intArray = {5,6,7,8};
    
    int sum = sumArray(intArray);
    
    System.out.println(sum);
    }
    
    public int sumArray(int[] myArray){
      int total = 0;
      
      for(int i = 0; i < myArray.length; i++){
        total = total + myArray[i];
      }
      
      return total;
    }     
}
```



