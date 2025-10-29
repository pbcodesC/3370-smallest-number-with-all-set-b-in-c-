# 3370-smallest-number-with-all-set-b-in-c-
class Solution {
public:
    int smallestNumber(int n) {
        int powerOfTwo = 1;
        while (powerOfTwo - 1 < n) {
            powerOfTwo <<= 1; // Equivalent to powerOfTwo *= 2
        }
        return powerOfTwo - 1;
    }
};
