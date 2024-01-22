//Array Programs...
public class SearchArray {
    //LINEAR SEARCH...
    /*public static int LinearSearch(int numbers[] , int key){
        for(int i=0;i<numbers.length;i++){
            if(numbers[i] == key){
                return 1;
            }
        }
        return -1;
    }
     public static void main(String[]args){
        int numbers[]= {34,67,12,78,90,23,45};
        int key=46;
        int index = LinearSearch(numbers, key);
        if(index==-1){
            System.out.println("Key is not found");
        }else{
            System.out.println("Key is found");
        }
        }*/
//LARGEST ELEMENT FROM ARRAY
        // public static void main(String[]args){
        //     int arr1[]=new int[]{6,78,34,23,90};
        //     int min = arr1[0];
        //     int max = arr1[0];

        //     for(int i=0;i<arr1.length;i++){
        //         if(arr1[i]<min){
        //             min=arr1[i];
        //         }
        //         if(arr1[i]>max){
        //             max=arr1[i];
        //         }
        //         System.out.println(min);
        //         System.out.println(max);

        //     }

        // }

        /*public static int getLargest(int numbers[]){
            int largest=Integer.MIN_VALUE;
            int smallest=Integer.MAX_VALUE;
            for(int i=0;i<numbers.length;i++){
                if(largest < numbers[i]){
                    largest=numbers[i];
                }
                if(smallest > numbers[i]){
                    smallest=numbers[i];
                }
            }
            System.out.println("Smallest value is:" +smallest);
            System.out.println("The Largest Number is:");
            return largest;
        }
        public static void main(String[]args){
            int numbers[]={6,78,23,12};
            System.out.println(getLargest(numbers));
        }*/

        //BINARY SEARCH
            /*public static int BinarySearch(int numbers[],int key){
            int start=0, end=numbers.length-1;
            while(start<=end){
                int mid=(start+end)/2;
                if(numbers[mid]==key){
                    return mid;
                }if(numbers[mid]<key){
                    start= mid+1;
                }else{
                    end = mid-1;
                }
            }
            return -1;
        }
         public static void main(String[]args){
            int numbers[]={34,78,90,12,45};
            int key=12;
            System.out.println(BinarySearch(numbers, key));
         }*/

         //REVERSE NUMBER IN GIVEN ARRAY 
         /*public static int ReverseNumber(int numbers[]){
            int first=0 , last=numbers.length-1;
            while(first<last){
                int temp = numbers[last];
                numbers[last]= numbers[first];
                numbers[first]=temp;
                first++;
                last--;
            }
            return last;
         }
         public static void main(String[]args){
            int numbers[]={4,5,6,78,12,};
            ReverseNumber(numbers);
            System.out.println("Reverese numbers from the array:");
            for(int i=0; i<numbers.length; i++){
            System.out.print(numbers[i] + " ");
            }
         }*/

         //PAIRS OF AN ARRAY
         /*public static void Printpair(int numbers[]){
            for(int i=0;i<numbers.length;i++){
                int curr = numbers[i];
                for(int j=i+1; j<numbers.length;j++){
                    System.out.print("(" +curr + "," +numbers[j] + ")");
                  }
                  System.out.println();
            }
         }
         public static void main(String[]args){
            int numbers[]={2,4,6,8,10};
            Printpair(numbers);    
         }*/

         //PRINT SUBARRAY
         /*public static void PrintSubarray( int numbers[]){
            for(int i=0;i<numbers.length;i++){
                int start =i;
                for(int j=i; j<numbers.length;j++){
                    int end=j;
                    for(int k=start; k<=end;k++){
                        System.out.print(numbers[k]+ " ");
                    }
                    System.out.println();
                }
                System.out.println();
            }
         }
         public static void main(String[]args){
            int numbers[]={2,4,6,8,10};
            PrintSubarray(numbers);
         }*/
         
         //MAX SUBARRAY SUM PRINTING...
         public static void MaxSubarraySum( int numbers[]){
            int currSum=0;
            int maxSum = Integer.MIN_VALUE;
            for(int i=0;i<numbers.length;i++){
                int start =i;
                for(int j=i; j<numbers.length;j++){
                    int end=j;
                    currSum=0;
                    for(int k=start; k<=end;k++){
                        currSum += numbers[k];
                    }
                    System.out.println(currSum);
                    if(maxSum<currSum){
                        maxSum = currSum;
                    }
                }
            
            }
            System.out.println("max sum is:" +maxSum);
         }
         public static void main(String[]args){
            int numbers[]={2,4,6,8,10};
            MaxSubarraySum(numbers);
         }
       }
       
