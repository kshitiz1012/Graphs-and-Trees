#include<bits/stdc++.h>
using namespace std;
 
 
#define ll long long
#define ld long double
#define endl "\n"
#define yes cout<<"YES"<<endl
#define no  cout<<"NO"<<endl
void solve()
{
     ll n,m;
     cin>>n>>m;
     ll dist[n+1][n+1];
     for(int i=1;i<=n;i++)
     {
          for(int j=1;j<=n;j++)
          {
               dist[i][j]=1e15;
               if(i==j)
               dist[i][j]=0;
          }
     }
     
          for(int i=0;i<m;i++)
          {
              ll first,second,third;
              cin>>first>>second>>third;
 
              dist[first][second]=min(dist[first][second],third);
              dist[second][first]=min(dist[second][first],third);
          }
 
     for(int k=1;k<=n;k++)
     {
          for(int i=1;i<=n;i++)
          {
               for(int j=1;j<=n;j++)
               dist[i][j]=min(dist[i][j],dist[i][k]+dist[k][j]);
          }
     }
}
int main()
{
     ll t=1;
	while(t--)
	{
	    solve();
	}  
	
}
