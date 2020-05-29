One of the main concept associated with normalization is **functional dependency**.
与规范化相关的一个主要概念是函数依赖性。

Functional Dependency: Describes the relationship between attributes in a relation. 
函数依赖:描述关系中属性之间的关系。

The main characteristics of functional dependencies that we use in normalization
我们在标准化中使用的函数依赖的主要特征:
– Have a one-to-one relationship between attribute(s) on left and right-hand side of a dependency;
在依赖项的左侧和右侧的属性之间具有一对一关系;
– hold for all time;
依赖关系一直存在
– are nontrivial.

一、部分函数依赖：
设X,Y是关系R的两个属性集合，存在X→Y，若X’是X的真子集，存在X’→Y，则称Y部分函数依赖于X。

例如：通过AB能得出C，通过A也能得出C，通过B也能得出C，那么说C部分依赖于AB。

二、完全函数依赖
设X,Y是关系R的两个属性集合，X’是X的真子集，存在X→Y，但对每一个X’都有X’!→Y，则称Y完全函数依赖于X。

例如：通过AB能得出C，但是AB单独得不出C，那么说C完全依赖于AB.

三、传递函数依赖
设X,Y,Z是关系R中互不相同的属性集合，存在X→Y(Y !→X),Y→Z，则称Z传递函数依赖于X。

例如：通过A得到B，通过B得到C，但是C得不到B，B得不到A，那么成C传递依赖于A