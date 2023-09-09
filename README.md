## Welcome to my  Pages

My QQ is 897224809. 

<div align="center"> <img src="https://metrics.lecoq.io/sun0225SUN?template=classic&config.timezone=Asia%2FShanghai"> </div>

And my e-mail: hanjingmin0805@gmail.com

### 

# 个人总结

- 主要研究传统图像处理方向, 例如图像去噪, 图像去模糊等
- 熟悉低秩矩阵分解, 稀疏编码, 张量矩阵运算等知识
- 编程语言python，熟练运用tensorflow,pytorch,keras等神经网络框架
- 熟悉c语言，数据结构，计算机网络
- 熟悉CNN（卷积神经网络）、RNN（循环神经网络）、强化学习等深度学习方法
- 团队精神，服从组织安排，有一定抗压能力，勤奋上进好学，吃苦耐劳，踏实肯干



​      

# 技能清单

以下均为我熟练使用的技能

- 计算机二级
- 熟练使用word、excel、powerpoint slide
- 编程语言：C/C++, python
- 版本管理、文档和自动化部署工具：Git
- 云和开放平台：微信应用开发
      

# 工作经历

## 2021年7月 ~ 2021年8月 

### ACM图灵大会 / 应急机动组组长
对组内志愿者进行工作安排, 落实组委会的相关任务,
负责对观众的疑问进行解答。

## 2019年9月 ~ 2022年6月 

### 异质物联网融合评价体系及评价方法 

项目描述：针对异质物联网互联实际需求, 从“数据-资源-服务”的角度, 设计评价体系, 规范异质互联评价指标和评价方法, 指导和评价异质互联模型、方法、架构和技术的设计。
本人工作：利用主成分分析等方法对构建异质物联网融合评价体系及评价方法。







# 个人信息

 - 韩靖敏/男/1995 
 - 本科/内蒙古大学数学学院 
 - 硕士研究生/合肥工业大学数学学院


 - Github：http://github.com/easychen ( 有原创repo的Github帐号会极大的提升你的个人品牌  )

 - 期望职位：算法工程师，开发岗
 - 期望薪资：税前月薪15k~20k，特别喜欢的公司可例外
 - 期望城市：北京、上海

# 指针进阶

## 数组

    数组：将具有同一属性的数据放在一起的有序集合。
    数组中的算法：求极值、排序、查找、求和等。
    主要类型：1.一维数组 2.多维数组  3.字符数组

### 一维数组

    一维数组定义的一般形式为 
        类型说明符  数组名[常量表达式] = { 初值表 };
    例如：
        int x[10] = { 0 };   /* 声明变量x中包含10个整型元素 */
    对所有元素赋初值需要注意:
    1-即使所有元素的值全部相同，也需要逐个赋值，不能给数组整体赋值。
    2-数值数组的赋值只能对数组元素逐一赋值，不能对数组名整体赋值。

#### 一维数组的应用

    题目： 求10个整型数中最大数、最小数以及所在位置的下标。
    程序实现：
        #include <stdio.h>
        int main(void)
        {
            int x[10] = { 31,6,1,48,4,2,4,3,15,32};
            int Max = x[0];
            int Min = x[0];
            int index_max,index_min;
            int i;
            for ( i = 0; i < 10; i++)
            {
    
                if (x[i] > Max)
                {
                    Max = x[i];
                    index_max = i;
                }
                else if (x[i] < Min)
                {
                    Min = x[i];
                    index_min = i;
                }
            }
            printf("第%d个元素为最大值%d，第%d个元素为最小值%d\n",index_max + 1,Max,index_min + 1,Min);
            return 0;
        }

### 多维数组

    多维数组定义的一般形式为：
        类型说明符  数组名[常量表达式1][常量表达式2]...[常量表达式n];
    以二维数组为例：
        int x[2][3] = { {1, 2, 3}, {4, 5, 6} };
    或  int x[2][3] = { 1, 2, 3, 4, 5, 6};

### 字符数组

    字符数组定义的一般形式为：
        字符类型说明符  数组名[常量表达式];
    例如：
        char s[] = {'P','r','o'};
    或
        char r[] = "pro";
    赋值后各元素的值为：
                        s[0]    s[1]    s[2]    s[3]
                         P       r       o      '\n'
    注意：s[]中系统在字符串常量末尾会自动加入空字符'\0'，实际的字符个数为3，这里按照数组定义长度为4，在标准中空字符不计入长度。

## 指针

0

## 指针数组

## 数组指针

## 函数指针

    指向函数指针！亦或存放函数地址的指针。
    数组的首元素地址&arr[0]与数组地址&arr是不同的。
    但函数名与函数地址表示是一致的。即   函数名 == &函数名
    
    一、(* (void(*)())0)();
        调用0地址出的函数
        该函数无参，返回类型是void
        1 - void(*)() ---- 函数指针类型
        2 - (void(*)())0 ---- 对0进行强制类型转换，可解释为一个函数地址
        3 - *(void(*)())0 ---- 对0地址进行解引用操作
        4 - (*(void(*)()0)() ---- 调用0地址处的函数
    
    二、void (* signal(int, void(*)(int)))(int);
        1 - signal和()先结合，说明siganl是函数名
        2 - signal函数的第一个参数的类型是int，第二个参数的类型是函数指针
            该函数指针，指向一个参数为int，返回类型是void的函数
        3 - signal函数的返回类型也是一个函数指针
            该函数指针，指向一个参数为int，返回类型是void的函数
            signal是一个函数的的声明

## 函数指针数组

    示例：
    #include <stdio.h>
    int Add(int x,int y)
    {
        return x + y;
    }
    int Sub(int x,int y)
    {
        return x - y;
    }
    int main(void)
    {
        int (* pf1)(int,int) = &Add;
        int (* pf2)(int,int) = &Sub;
        int (* pfArr[2])(int,int) = {Add,Sub};
    
        return 0;
    }

## 指向函数指针数组的指针

     void (*(*pArr)[5])(int) = &Arr

## 回调函数

    定义：回调函数就是一个通过函数指针调用的函数。如果你把函数的指针(地址)作为参数传递给另一个函数，当这个指针被用来调用其所指向的函数时，我们就说这是回调函数。回调函数不是由该函数的实现方直接调用，而是在特定的时间或条件发生时由其他函数方法调用。




## 结构体

### 结构体类型的声明

#### 结构的基础知识 

结构是一些值的几何，这些值称为成员变量。结构的每个成员可以是不同类型的变量。

#### 结构体的声明

    struct tag
    {
        memeber-list;
    }variable-list;
    例如描述一个学生的结构体类型为；
    struct Stu
    {
        char name[20];  // 结构体变量
        char sex[10];
        char tele[12];
        int age;
    }s3,s4,s5;     // s1,s2,s3,s4,s5均为全局变量，两种不同的声明方式
    结构体变量的创建：
    struct Stu s1;
    struct Stu s2;
    注：匿名结构体类型

### 结构的自引用

    以链表为例，分布在不连续内存中的五个数字 1，2，3，4，5
    思考，若利用一下结构体定义，是否可行？
    struct Node
    {
        int value;    // 链表需要指针 value next 三个要素
        // struct Node n; // sizeof(Struct Node) 占用无限多的内存
        struct Node* next; // 4/8字节
    }
    
    typedef 对类型进行重命名
    typedef struct Node
    {
        int value;    
        struct Node* next; 
    }Node;
    将结构体类型重新命名为Node类型
    int main(void)
    {
        struct Node n1;     // 可
        Node n2;            // 可
    
        return 0;
    }
    当使用匿名结构体类型时，需注意
    typedef struct 
    {
        int value;    
        Node* next;  // struct Node* next;错误 
        // 第一次定义过程中 Node类型不存在，完整执行后才会命名Node
        // 所以typedef struct Node不能丢
    }Node;

### 结构体变量的定义和初始化

    struct T   // 结构体变量的定义
    {
    
        double weight;
        double height;
     
    };
    struct S    // 结构体变量的定义
    {
        char c;
        int a;
        struct T t;
        double d;
        char arr[20];   
    };
    // 初始化
    int main(void)
    {
        struct S s = { 'c', 100,{178.0,160.0}, 3.14, "hanmingmin@gamil.com"};     // 结构体变量声明
        printf("%c %d %lf %lf %lf %s",s.c,s.a
            ,s.t.weight,s.t.height,s.d,s.arr);          
    
        return 0;
    }

### 结构体的内存对齐

    struct S1    // 结构体变量的定义
    {
        char c1;
        int a;
        char c2;
    };
    struct S2    // 结构体变量的定义
    {
        char c1;
        char c2;
        int a;
    };
    // 初始化
    int main(void)
    {
        struct S1 s1 = {0};     // 结构体变量声明
        printf("%ld\n",sizeof(s1));          
        struct S2 s2 = {0};     // 结构体变量声明
        printf("%ld\n",sizeof(s2));   
        return 0;
    }    

### 结构体传参

### 结构体实现位段(位段的填充&可移植性)

## 枚举

### 枚举类型的定义

### 枚举的优点

### 枚举的使用

## 联合

### 联合类型的定义

### 联合的特点

### 联合大小的计算

