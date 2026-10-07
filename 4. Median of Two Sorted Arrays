 /*
Given two sorted arrays nums1 and nums2 of size m and n respectively, return the median of the two sorted arrays.

The overall run time complexity should be O(log (m+n)).

Example 1:

Input: nums1 = [1,3], nums2 = [2]
Output: 2.00000
Explanation: merged array = [1,2,3] and median is 2.
Example 2:

Input: nums1 = [1,2], nums2 = [3,4]
Output: 2.50000
Explanation: merged array = [1,2,3,4] and median is (2 + 3) / 2 = 2.5.
 
Constraints:

nums1.length == m
nums2.length == n
0 <= m <= 1000
0 <= n <= 1000
1 <= m + n <= 2000
-106 <= nums1[i], nums2[i] <= 106
*/

class Solution {
public:
    double findMedianSortedArrays(vector<int>& nums1, vector<int>& nums2) {
        double abs  ;
        vector<int>nums3 = nums1;
        for (int i = 0; i < nums2.size(); i++) {
            nums3.push_back(nums2[i]); 
        }
        int n =nums3.size();
        sort(nums3.begin(), nums3.end());
        if(nums3.size()%2 ==0){
            int i = nums3[(n/2)-1] +nums3[(n/2)];
            abs = i/2.0;
        }
        else if(n ==1){
            abs = nums3[0];
        }
        else{
             abs=nums3[(n/2)] ;
        }
        return abs;
    }
};
