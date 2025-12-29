def findMaxConsecutiveOnes(nums):
    count = 0      # counts current 1s
    max_count = 0  # stores maximum 1s

    for num in nums:
        if num == 1:
            count += 1
            max_count = max(max_count, count)
        else:
            count = 0   # reset when 0 comes

    return max_count

