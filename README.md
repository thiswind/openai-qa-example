# openai-qa-example

## 依赖
```bash
pip install openai
```

## 运行示例

```text
    $ export OPENAI_API_KEY=你的OpenAI的API Key

    $ python qa_ai.py -q "请给我一个冒泡排序函数 的例子。"
    You asked: 请给我一个冒泡排序函数的例子。
    AI answered: 
    AI: 你可以使用这个Python函数来实现冒泡排序：
    ```
    def bubble_sort(arr):    
        n = len(arr)
        
        # 在range(n)中的每一个i，都不断检查arr[i]和arr[i+1]
        for i in range(n):
            # 如果arr[i]>arr[i+1]，那么就交换它们的位置
            for j in range(0, n-i-1):
                if arr[j] > arr[j+1]:
                    arr[j], arr[j+1] = arr[j+1], arr[j]
                    
    arr = [14,46,43,27,57,41,45,21,70]
    bubble_sort(arr)
    
    print ("排序后的数组:")
    for i in range(len(arr)):
        print ("%d" %arr[i]),
    ```
```
