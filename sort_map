class Solution {
public:
      static bool cmp(pair<int,int> &l, pair<int, int> &r) {
        if (l.second == r.second)
            return l.first > r.first;
        return l.second < r.second;
    }
    vector<int> frequencySort(vector<int>& nums) {
     unordered_map<int,int> m;
        vector<int> k;
        for(int i=0;i<nums.size();i++) {
            m[nums[i]]++;
        }
         vector<pair<int,int>> v(m.begin(), m.end());
        sort(v.begin(), v.end(),cmp);
for(auto &it:v) {
    while (it.second > 0) {
        k.push_back(it.first);
        it.second-=1;
    }
