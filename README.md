# Unique-Number-of-Occurrences
class Solution:
    def uniqueOccurrences(self, arr: List[int]) -> bool:
        count=Counter(arr)
        for i,c1 in count.items():
             for j,c2 in count.items():
                if i!=j and c1==c2:
                    return False
        return True
