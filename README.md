# 计算机二级笔记 

### 二叉数的遍历
> **前序遍历**：根结点 ---> 左子树 ---> 右子树   
**中序遍历**：左子树 ---> 根结点 ---> 右子树    
**后序遍历**：左子树 ---> 右子树 ---> 根结点   

![二叉数遍历](./1.png)    

> **前序遍历**：1  2  4  5  7  8  3  6    
**中序遍历**：4  2  7  5  8  1  3  6    
**后序遍历**：4  7  8  5  2  6  3  1

### 程序的执行方式
1. **顺序**执行
    - **可再现性**             
        处理机严格地按照程序所规定的顺序执行，即每一操作必须在下一个操作开始之前结束
    - **封闭性**         
        程序在封闭的环境下运行，即程序运行时独占全机资源，资源的状态（除初始状态外)只有本程序才能改变它，程序一旦开始执行，其执行结果不受外界因素影响
    - **可再现性**           
    指只要程序执行时的环境和初始条件相同，当程序重复执行时，不论它是从头到尾不停顿地执行，还是“停停走走”地执行，都可获得相同的结果程序顺序执行时的这种特性，为程序员检测和校正程序的错误带来了很大的方便
2. **并发**执行
    - **间断性**        
    程序在并发执行时，由于它们共享系统资源，以及为完成同一项任务而相互合作，致使在这些并发执行的程序之间形成了相互制约的关系。相互制约将导致并发程序具有“执行-暂停-执行”这种间断性的活动规律。
    - **失去封闭性**          
    当系统中存在着多个可以并发执行的程序时，系统中的各种资源将为它们所共享，而这些资源的状态也由这些程序来改变，致使其中任一程序运行时，其环境都必然受到其他程序的影响。
    - **不可再现性**           
    程序在并发执行时，由于失去了封闭性，其计算结果必将与并发程序的执行速度有关，从而使程序的执行失去了可再现性。换而言之，程序经过多次执行后，虽然它们执行时的环境和初始条件相同，但得到的结果却各不相同。