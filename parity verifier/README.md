奇偶校验

  奇偶校验是一种简单、实现代价小的检错方式，常用在数据传输过程中。对于一组并行传输的数据（通常为8比特），可以计算岀它们的奇偶校验位并与其一起传输。接收端根据接收的数据重新计算其奇偶校验位并与接收的值进行比较，如果二者不匹配，那么可以确定数据传输过程中岀现了错误；如果二者匹配，可以确定传输过程中没有出错或者出现了偶数个 错误(出现这种情况的概率极低)。奇偶校验包括奇校验和偶校验两种类型。

偶校验和奇校验

  对于偶校验，包含校验比特在内，1的总数是偶数。在奇校验中，1的总数则为奇数。
 
  例如:

data\_in[7:0]=1010\_1011

  在该数据串中有5个1，偶校验时，校验结果为1，这样1的总个数为偶数；在奇校验时，校验比特为0,使得1的总个数为奇数。又如：

data\_in[7:0]=0000\_1111

  在该数据串中有4个1，偶校验时，校验结果为0,使得1的总个数仍为偶数；在奇校验时，校验比特为1，使得1的总个数为奇数。
