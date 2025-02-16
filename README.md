# array3
1 Triplets in the array adds up to the target
// Online Java Compiler
// Use this editor to write, compile and run your Java code online

class Main {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        int count=0;
        int target = 12;
        int[] arr = {1,4,5,6,3}; 
        for(int i=0;i < (arr.length-2);i++){
            for(int j=i+1;j<(arr.length-1);j++){
                for(int k=j+1;k<(arr.length);k++){
                if(arr[i]+arr[j]+arr[k]==target){
                    count++;
                }
                }
            }
        }
        System.out.println("The number of Triplets Possible is "+count);
        
    }

    2.Finding the unique element present in the given array

    // Online Java Compiler
// Use this editor to write, compile and run your Java code online

class Main {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        int count=0;
        boolean isUnique;
        int[] arr = {1,2,3,4,2,1,3}; 
        for(int i=0;i < arr.length;i++){
            isUnique = true;
            for(int j=0;j<arr.length;j++){
                if(i!=j && arr[i]==arr[j]){
                    isUnique = false;
                    break;
                }
                }
                if(isUnique){
                    System.out.println("The unique element is "+arr[i]+" present at the location "+i);
            }
        }
        
        
    }
}
#alternative to this is, just traverse through the array and change to -1 , for all which has its pair, and then traverse the array and return the one which is not -1

3.Program to find the second largest element in the Given Array
sort first and then return the last but second element(limitations if maximum has multiple , occurances then this fails)
•Or find the maximum and make its appereace -1 , and then find maximum again
•Integer.MINVALUE, Integer.MAXVALUE


4.Given An array return the first element which is repeating
•class Main {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");

        int[] arr = {1, 2, 3, 4, 2, 1, 3, 4, 6, 6, 7, 8, 9, 8}; 
        boolean found = false;

        for (int i = 0; i < arr.length; i++) {
            for (int j = i + 1; j < arr.length; j++) {
                if (arr[i] == arr[j]) {  // Found a repeating element
                    System.out.println("The first repeating element is " + arr[i] + " found at index " + i);
                    found = true;
                    break;
                }
            }
            if (found) break;  // Exit the loop after finding the first repeating element
        }

        if (!found) {
            System.out.println("No repeating elements found.");
        }
    }
}


5. Given an array give ,last repeating element
6. Given an array return the second smallest element

}
