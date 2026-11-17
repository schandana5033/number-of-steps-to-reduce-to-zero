# number-of-steps-to-reduce-to-zero
class Solution {
    public int numberOfSteps(int num) {
        int steps = 0;
        while (num > 0) {
            if (num % 2 == 0) num /= 2;
            else num--;
            steps++;
        }
        return steps;
    }
}
// Time: O(log n) | Space: O(1)
