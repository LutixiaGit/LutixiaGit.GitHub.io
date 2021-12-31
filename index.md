## Welcome To Qian's Page



https://user-images.githubusercontent.com/78092087/147802057-0a9f3a38-87a7-4816-a869-a872e1f1b5a0.mp4



### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block
#include<iostream>
using namespace std;
const int N=100+5;//物品种类 
const int M=100+5;//背包大小 
int a[N][2];//第二维0是所占空间 1是拥有价值 
int dp[M];
int main()
{
	int n, m;
	cin>>m>>n;
	for(int i = 1; i <= n; i++)
		cin>>a[i][0]>>a[i][1];	
	for(int i = 1; i <= n; i++)
		for(int j = m; j >= a[i][0]; j--)
			dp[j] = max(dp[j], dp[j-a[i][0]] + a[i][1]);
	cout<<dp[m]<<endl; 
	return 0;
}
[Link](url) and ![Image](src)
```
