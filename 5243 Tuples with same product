class Solution:
    def tupleSameProduct(self, nums: List[int]) -> int:
        n = len(nums)
        productfreq = dict();
        for i in range(n - 1):
            for j in range(i + 1, n):
                product = nums[i] * nums[j]
                productfreq[product] = productfreq.get(product, 0) + 1
        ans = 0
        for k, v in productfreq.items():
            ans += v * (v - 1) / 2


        return int(ans * 8)
