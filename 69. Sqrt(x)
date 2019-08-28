class Solution {
    public int mySqrt(int x) {
        if (x < 2) {
            return x;
        }
        long num;
        int pivot, left = 2, right = x / 2;
        while (left < right - 1) {
            pivot = left + (right - left) / 2;
            num = (long)pivot * pivot;
            if (num == x) {
                return pivot;
            } else if (num < x) {
                left = pivot;
            } else {
                right = pivot - 1;
            }
        }
        return (long)right * right <= x ? right : left;
    }
}