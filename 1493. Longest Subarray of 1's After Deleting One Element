public class Solution {
    public int LongestSubarray(int[] arr) {
        List<int>zeros=new List<int>();
        for (int i=0;i<arr.Length;i++){
            if(arr[i]==0){
                zeros.Add(i);
                Console.WriteLine(i);
            }
        }
        if (zeros.Count<=1)
        return arr.Length-1;
        zeros.Add(arr.Length);
        int res=zeros[1]-1;
        for (int i=1;i<zeros.Count-1;i++){
            res=Math.Max(res,(zeros[i+1]-zeros[i]-1)+(zeros[i]-zeros[i-1]-1));
        }
        return res;
    }
}
