# Valid Palindrome (easy)

```python
class Solution:
    def isPalindrome(self, s: str) -> bool:
        new_string = [string for string in s if string.isalnum()]
        clean_string = "".join(new_string).lower()
        print(clean_string)
        start = 0
        end = len(clean_string) - 1
        while start <= end:
            if clean_string[start] != clean_string[end]:
                return False
            start += 1
            end -= 1
        return True

```
