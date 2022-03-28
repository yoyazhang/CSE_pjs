# Part A

- 计算机系统的可靠性指在规定条件下和给定时间内计算机系统正确运行、不出错、不损坏的概率。
- 例本课程Lab1的文件系统中通过将同一份数据冗余地存储在n个block中来保证一个block损坏后系统仍能通过对应损坏块的meta中duplicate blocks记录找到冗余块、返回正确的内容；同时更加保证了计算机系统可靠性的方法是另开一个新的线程去进行定时的检查、恢复那些被损坏的重复块，保证其以最高的概率正常运行(前者可能会出现全部冗余块都损坏后、文件也彻底损坏的情况)