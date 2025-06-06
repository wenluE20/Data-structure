# 1002 用数组实现栈的基本操作

用数组实现栈的基本操作，包括：

  （1）Push 将元素压入栈顶

  （2）Pop 获取并移除栈顶元素

  （3）GetTop 获取栈顶元素

  （4）StackEmpty 判断栈是否为空

# 输入输出格式
单次输入一行为一个独立的指令，一行中是一个或几个整型参数，用空格隔开。第一个参数是指令，0-3对应上述四种操作，-1表示退出程序。

（1）Push 将元素压入栈顶

  **输入：第二个参数为操作次数，后续参数为数据**
  
  0 7 0 1 2 3 4 5 6  /*入栈7次，数据为0、1、2、3、4、5、6*/
  
  **输出：栈的全部元素（自栈顶至栈底，用空格隔开）**
 
  Stack: 6 5 4 3 2 1 0

（2）Pop 获取并移除栈顶元素

  **输入：第二个参数为操作次数**
  
  1 2  /*连续两次将栈顶元素弹出栈并获取*/
  
  **输出：弹出的栈顶元素和栈的剩下元素（栈顶至栈底，用空格隔开）**
  
  // 弹出成功
  Pop: 6  /*依次弹出栈顶元素6、5*/
  Stack: 5 4 3 2 1 0
  Pop: 5
  Stack: 4 3 2 1 0
  
  // 弹出失败
  Pop failed  /*失败了几次就会打印几次该信息*/

（3）GetTop 获取栈顶元素

  **输入：**
  
  2  /*获取栈顶元素，而不弹出*/
  
  **输出：栈顶元素和栈的剩下元素（栈顶至栈底，用空格隔开）**
  
  // 获取成功
  GetTop: 4
  Stack: 4 3 2 1 0
  
  // 获取失败
  GetTop failed

（4）StackEmpty 判断栈是否为空

  **输入：**
  
  3  /*判断栈是否为空*/
  
  **输出：**
  
  // 栈空
  
  The Stack is Empty
  
  // 栈非空
  
  The Stack is not Empty
  
  Stack: 4 3 2 1 0

