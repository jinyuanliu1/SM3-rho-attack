# SM3-rho-attack
原理很简单，我们只需要从一个初始值出发，不断计算SM3值，就可能成环（前n bit），在代码中可以参考Floyd判环法
在实验中，我们可以调节碰撞的比特数，8bit时，计算十分快速，而当比特数到达24bit时，受我们添加的随机的字符串的影响就比较大了，有些很快，有些很慢，当比特数到达32bit时，运行就有些缓慢了
