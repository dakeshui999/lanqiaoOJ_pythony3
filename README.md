# lanqiaoOJ_pythony3
三角回文数（山）
#题目
#12356321,145541，它们左右对称（回文）且数位上的数字先单调不减，后单调不增。在[2022,2022222022]中有多少个数形状像一座山。
ans = 0    #ans是anwser
for i in range(20,20223):         #回文串长度是偶数，右半边是左半边的翻转
  flag = 1
  s = str(i)
  for i in range(0,len(s)):       #判断左半边的单调性
    if s[i] >s{i+1}:              #非单调不减
      flag = 0                    # = 0：不合法
      break
  if flag == 1:
    ans += 1
for i in range(11,10000):         #得到了左半边，可以构造一个“山”数
  flag = 1                        #[11,9999]。回文串长度为奇数，中间数不小于左右两边
  s = str(i)
  for i in range(0,len(s)-1）:    #     
    if s[i] > s[i+1]:
        flag = 0
        break
  if flag == 1:
      ans += 10 - int(s[i+1])
print(ans)
#对于正整数n，如果存在正整数k使得n = 1+2+3+4+5+6+7+8+9........k=k(k+1)/2,则n称为三角数。第一个大于20220514的三角回文数是多少？
for k in range(4000,20000):
    n = k *(k+1)//2
    s = str(n)
    if s[::-1]==s:
          print(k,n);
          break

