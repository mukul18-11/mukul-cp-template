#include <iostream>       // cin, cout, cerr
#include <vector>         // vector
#include <string>         // string
#include <algorithm>    
#include <cmath>        
#include <climits>      
#include <cfloat>         
#include <cstdlib>        
#include <ctime>          
#include <chrono>         
#include <random>         
#include <unordered_map>  
#include <set>            
#include <map>            
#include <queue>        
#include <stack>         
#include <deque>          
#include <bitset>        
#include <utility>       
#include <functional>    
#include <cstring>        
#include <cassert>        
#include <cstdio>         

#define ios ios_base::sync_with_stdio(false);cin.tie(NULL)

#define ll long long
#define ld long double
#define pb push_back
#define mp make_pair
#define vi vector<int>
#define vl vector<ll>
#define vc vector<char>
#define vvc vector<vc>
#define vm vector<modint>
#define vvi vector<vi>
#define vvl vector<vl>
#define vvm vector<vm>
#define pii pair<int, int>
#define pll pair<ll, ll>
#define pmm pair<modint, modint>
#define vpii vector<pii>
#define vpll vector<pll>
#define vpmm vector<pmm>
#define mem1(a)          memset(a,-1,sizeof(a))
#define mem0(a)          memset(a,0,sizeof(a))
#define ppc              __builtin_popcount
#define ppcll            __builtin_popcountll

#define f first
#define s second

#define all(v) v.begin(), v.end()
#define rall(v) v.rbegin(), v.rend()

#define foi(i,n) for(ll i = 0 ; i < n ; i++)
#define rfoi(i,n) for(ll i = n ; i > 0 ; i--)
#define rep(i,a,b,c) for(ll i=a;i<b;i+=c)

#define inputk(v) ll n, k; cin>>n>>k; vector<ll> v(n); for (ll i = 0; i < n; i++) {cin>>v[i];}
#define input(v) ll n; cin>>n; vector<ll>v(n); for (ll i = 0; i < n; i++) {cin>>v[i];}

#define inputvfreq unordered_map<ll,ll> freq; foi {freq[v[i]]++;}

#define tc ll t; cin>>t; while(t--)

#define inputmat(mat,n,m) ll n,m; cin>>n>>m; \
vector<vector<ll>> mat(n, vector<ll>(m)); \
for(ll i = 0; i < n; i++) \
for(ll j = 0; j < m; j++) \
cin >> mat[i][j];

using namespace std;

mt19937_64 RNG(chrono::steady_clock::now().time_since_epoch().count());

int findDigSum(int n, int sum){
    if(n == 0)return sum;
    return  findDigSum(n/10, sum + (n % 10));
}

int main(){
    auto begin_time = chrono::high_resolution_clock::now();
    ios;

    #ifndef ONLINE_JUDGE
        freopen("input1.txt","r",stdin);
        freopen("output1.txt","w",stdout);
    #endif 

        // your code starts here 
        tc{
            int n ; cin >> n ; 
            vector<string> s(n,0);
            for(int i = 0 ; i < n ; i++){
                cin>>s[i]>>endl;
            }
        }



        // your code ends here 


    auto end_time = chrono::high_resolution_clock::now();
    auto elapsed = chrono::duration_cast<chrono::nanoseconds>(end_time - begin_time);
    cerr << "Time measured: " << elapsed.count() * 1e-9 << " seconds." << endl;

    return 0;
}
