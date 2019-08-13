# 基本知识和语法

1. 关于变量
      - ```kotlin
        Var name: String="" 
        ```

      - Var 变量 val不可变 

      - 可以不加type，赋值后不能变type 

    - 值为null的变量声明时： 

      - ```kotlin
        Val name: type?=null 
        ```

2. When 语法

      ```kotlin
      when(x){
          1 -> ("x==1")
          3,4 -> print("sss")
          5...10 -> print("")
          "string" -> print("")
          else -> {
              ...
          }
      }
      ```

      

3. 函数

      ```kotlin
      fun funcName(): returnType {
      	return something
      }
      ```

      

4. "$"符号提示变量 

   ```kotlin
   var varName
   val newVar = "some $varName"
   ```

5. 数组

   ```kotlin
   var array = arrayOf("a","b","c")
   ```

6. For 循环和 forEach

   ```kotlin
   for (i in array){
   	opration(i)
   }
   ```

   ```kotlin
   array.forEach { it ->
   	operation(it)
   }
   ```

7. Map

      ```kotlin
      val map = mapOf(1 to "a")
      map.forEach{key, value -> print("$key -> $value")}
      ```

8. List

      ```kotlin
      val list = listOf("a","b")
      ```

9. Collection 有两种，一种不可变，一种mutable

10. vararg 用于参数个数可以变化的情况

      ```
      fun variableParaNum(vararg arg){}
      
      fun main(){
      	val a = listOf("a","b")
      	variableParaNum("a","b")
      	variableParaNum(*a)
      }
      ```

      