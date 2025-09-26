class Solution {
 #define ll long long
public:
    int pivotIndex(vector<int>& a) {
        ll total_sum = accumulate(a.begin(), a.end(), 0);
        ll ans = -1;
        ll left_sum = total_sum, right_sum = 0;

        for(int i = a.size() - 1 ; i >= 0 ; i--) {
            left_sum = left_sum - a[i];

            if(left_sum == right_sum) {
                ans = i;
            }

            right_sum += a[i];
        }

        return ans;
    }
};
