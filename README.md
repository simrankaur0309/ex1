# ex1
#include &lt;cmath> #include &lt;cstdio> #include &lt;vector> #include &lt;iostream> #include &lt;algorithm> using namespace std; typedef long long int ll;  ll permute(string str,ll b)  {      // Sort the string in lexicographically      // ascennding order      sort(str.begin(), str.end());      ll max=0;     // Keep printing next permutation while there      // is next permutation      do {                 if(stoll(str)&lt;b&amp;&amp;stoll(str)>max)             max=stoll(str);     } while (next_permutation(str.begin(), str.end()));      return max; }  int main() {     string a;      ll b;/* Enter your code here. Read input from STDIN. Print output to STDOUT */         cin>>a>>b;      ll ans=permute(a,b);      cout&lt;&lt;ans&lt;&lt;endl;     return 0; }
