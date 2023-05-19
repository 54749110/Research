<style>

H1 {font-family: "times new Roman", "宋体"}
h1 {font-size: 30px}
h1 {font-weight: bold}

H2 {font-family: "times new Roman", "楷体"}
h2 {font-size: 20px}
h2 {color: rgb(0,0,153)}
h2 {font-weight: bold}
h2 {margin-top: 30px}
h2 {margin-bottom:0px}

H3 {font-family: "times new Roman", "楷体"}
h3 {font-size: 20px}
h3 {color: rgb(0,0,153)}
h3 {font-weight: bold}

p {font-family: "times new Roman", "宋体"}
p {font-size: 12px}
p {font-weight: bold}
p {line-height: 150%}


blockquote p {padding-left: 5px; 
  padding-top: 8px;
  padding-bottom: 8px;
  font-size: 11px}

blockquote  {
  background-color: rgb(235,235,235); 
  border-left-style:solid;
  border-left-width:2px ;
  border-color:rgb(51,153,255)}

%%非全局格式
<font color=red>我是红色</font>

%%添加图片,center指的图片居于文字外，不要改
<img src="./xxx.png" width = "300" height = "200" alt="图片名称" align=center />

%% run command "create table of contents" 添加目录

</style>

# <center> Ring exchange model
REF  
[[1]](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.72.115114)J.-Y. P. Delannoy, M. J. P. Gingras, P. C. W. Holdsworth, and A.-M. S. Tremblay,Néel order, ring exchange, and charge fluctuations in the half-filled Hubbard model ,Phys. Rev. B 72, 115114 (2005)    
[[2]](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.37.9753)A. H. MacDonald, S. M. Girvin, and D. Yoshiokat, t/U expansion for the Hubbard model,Phys. Rev. B 37, 9753 (1988)




##  正则变换(canonical transformation)求解高阶哈密顿量
---
&emsp;&emsp;四费米子之间的相互作用是有趣的，然而我们一般讨论的哈密顿量只包括二费米子。我们以半充满的Hubbard(t-J)模型为例，得到 t-J模型有几种方法，一种就是曾经提到的投影矩阵的方法，即：


&emsp;&emsp;写出矩阵元之后，就可以求解能量本征方程利用单占据条件<n>=1就可以得到半充满的哈密顿量了。 另一种方法是我们在从Anderson Impurity Model求解Kondo的哈密顿量中所用的Schrieffer-Wolff 变换，即利用正则变换矩阵S将Anderson Hamiltonian 投影去除了跃迁项，再通过单占据条件得到了以单占据态为主导的Kondo Hamiltonian。这里我们用类似的方法处理Hubbard Hamiltonian 。不同的是，在处理Kondo Hamiltonian的时候我们只保留了哈密顿量的零阶项与二阶项，这里为了得到四费米子的项，我们需要保留更高阶的项。对Hubbard Hamiltonian做如下的分解: +1双占据态，-1双占据态，双占据态数目不变。


&emsp;&emsp;这正是增加双占据态的表述。根据Schrieffer-Wolff 变换，一阶S矩阵的目的就是要消除+1项与-1项，然而正如我们在Kondo Hamiltonian中看到的，这不可避免会在引入二阶小量，我们再用三阶S矩阵消去二阶小量就得到了所要求的四阶哈密顿量,如下：

&emsp;&emsp;具体推导过程可见附录。上面的讨论排除了一次哈密顿量的非单占据态，而对于四阶哈密顿量，还需要排除在同阶U下面的其它非单占据态，具体来说，有以下三种：