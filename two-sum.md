[Two Sum](https://leetcode.com/problems/two-sum/)

## GO

```go
func twoSum(nums []int, target int) []int {

    for i, num1 := range nums {
        for j, num2 := range nums {
            if i != j {
                if num1 + num2 == target {
                    return []int{i, j} 
                }
            }
        }
    }               
    
    return []int{} 
}
```

## JS

```js
var twoSum = function(nums, target) {
    if (nums === null || target === undefined || target === null || target === undefined  || nums.length < 2) return;
    
    for (var i = 0; i < nums.length - 1; i++) {
        for (var j = i+1; j < nums.length; j++) {
            if (nums[i] + nums[j] === target) return [i, j];
        }
    }
};
```
