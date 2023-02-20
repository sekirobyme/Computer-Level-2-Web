# 计算机二级笔记 

# 目录
## [树](#tree)
## [算法](#算法)  
## [栈](#栈)  
## [队列](#队列)  
## [数据库](#数据库)

## <a id="tree">树</a>
树是n（n>=0）个结点的有限集        

1. 树中一个结点的孩子个数称为该结点的度,树中结点的最大度数称为树的度    .    
2. 度大于0的结点称为分支结点(又称非终端结点);度为0(没有子女结点)的结点称为叶子结点(又称终端结点)。在分支结点中,每个结点的分支数就是该结点的度。
3. - 结点的深度是从根结点开始自顶向下逐层累加的。
   - 结点的高度是从叶结点开始自底向上逐层累加的。
   - 树的高度(或深度)是树中结点的最大层数。
4. 有序树和无序树。树中结点的各子树从左到右是有次序的,不能互换,称该树为有序树,否则称为无序树
5. 路径和路径长度。树中两个结点之间的路径是由这两个结点之间所经过的结点序列构成的,而路径长度是路径上所经过的边的个数。
6. 森林。森林是m(m≥0)棵互不相交的树的集合。

    #### 树的性质
    1. 树中的结点数等于所有结点的度数加1.
    2. 度为m的树中第i层上最多有m<sup>i-1</sup>个节点(i>=1)。
    3. 高度为h的m叉树至多有(m<sup>h</sup>-1)/(m-1)个结点。
    4. 具有n个结点的m叉数的最小高度为[log<sub>m</sub><sup>(n(m-1)+1)</sup>]  


### 二叉树
#### 二叉数的遍历
> **前序遍
![二叉数遍历](./1.png)    

> **前序遍历**：1  2  4  5  7  8  3  6    
**中序遍历**：4  2  7  5  8  1  3  6    
**后序遍历**：4  7  8  5  2  6  3  1历**：根结点 ---> 左子树 ---> 右子树   
**中序遍历**：左子树 ---> 根结点 ---> 右子树    
**后序遍历**：左子树 ---> 右子树 ---> 根结点   

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
    
## 算法<a id="Algorithm"></a>
### 算法的复杂度
- 复杂度分析   
通常一个算法的复杂度是由其输入量决定的
- 时间复杂度      
执行算法所需要的计算工作量
- 空间复杂度     
算法在计算机内执行时所需存储空间的度量

## 栈
只允许在一端进行插入或删除操作的线性表。首先，栈是一种线性表，但限定这种线性表只能在某一段进行插入和删除操作。

栈顶（**Top**）：线性表允许进行插入和删除的一端。

栈底（**Bottom**）：固定的，不允许进行插入和删除的另一端。

空栈：不含任何元素。   

![栈](./2.jfif)

栈空条件：S.top == -1

栈满条件：S.top == MAXSIZE - 1

栈长：S.top + 1

## 队列
一种特殊的线性表,它只允许在表的前端（front）进行删除操作，而在表的后端（rear）进行插入操作。进行插入操作的端称为队尾，进行删除操作的端称为队头。队列中没有元素时，称为空队列。


#### 结构化程序设计和结构化程序设计方法 
结构化程序设计适用于程序规模较大的情况，对于规模较小程序也可采用非结构化程序设计方法。       
1.  - 结构化程序设计是进行以**模块功能**和**处理过程**设计为主的详细设计的基本原则
    - 结构化程序设计方法是按照模块划分原则以提高程序**可读性**和**易维护性**、**可调性**和**可扩充性**为目标的一种程序设计方法
2. 原则
    - 自顶向下
    - 逐步细化
    - 模块化
    - 结构化编码
   
    
    
    
## 数据库

### 数据库管理技术发展的三个阶段
1. 人工管理阶段   
20世纪50十年代中期以前，计算机主要用于科学计算，由**人工**进行数据管理。
2. 文件系统管理阶段   
20世纪50年代后期到60年代中期，这时硬件方面有了磁盘、磁鼓等直接存取存储设备；软件方面，操作系统中已经有了专门的数据管理软件。一般称为文件系统，处理方式上不仅有批处理，而且能够联机实时处理。
3. 数据库系统阶段   
20世纪60年代，这时硬件已有大量容量磁盘，硬件价格下降，软件价格上升。处理文件方式上，人们越来越需要联机实时处理。在这种背景下就诞生了统一管理数据的专门软件系统——数据库管理系统。

#### E-R图(实体-联系模型)
实体：客观存在且可以互相区别的事物。
属性：实体的特征描述。