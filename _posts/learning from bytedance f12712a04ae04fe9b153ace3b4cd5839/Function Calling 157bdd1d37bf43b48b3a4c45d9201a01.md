# Function Calling

https://luxiangdong.com/2024/04/13/func-call/

![Untitled](Function%20Calling%20157bdd1d37bf43b48b3a4c45d9201a01/Untitled.png)

1. 用户向应用程序提出问题
2. 应用程序传递用户提供的prompt和函数声明，这是对模型可以使用的工具的描述
3. 根据函数声明，模型建议要使用的工具以及相关的请求参数。**请注意，模型仅输出建议的工具和参数，而不实际调用函数**
4. 4 & 5 根据响应，应用程序调用相关 API
5. 6 & 7 来自 API 的响应再次输入模型，模型再输出人类可读的响应
6. 应用程序将最终响应返回给用户，然后从 1 开始重复。

![Untitled](Function%20Calling%20157bdd1d37bf43b48b3a4c45d9201a01/Untitled%201.png)