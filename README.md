# pair-sum
//You have been given an integer array/list(ARR) and a number X. Find and return the total number of pairs in the array/list which sum to X.
int pairSum(int *input, int size, int x)
{
    int countpair=0;
   for(int i=0;i<size;i++){
       for(int k=i+1;k<size;k++){
            if(input[i]+input[k]==x){
               countpair++;
           }
       }
   }
    return countpair;
}
