# This is an `<h1>` header, which is the largest

## This is an `<h2>` header

###### This is an `<h6>` header, which is the smallest
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
``` c++
#include<bits/stdc++.h>
using namespace std;
#define M 1000000007
#define ll long long
typedef long double ld;
#define pb push_back
#define is insert
#define f first
#define s second
#define all(a) a.begin(), a.end()
#define rall(a) a.rbegin(), a.rend()
typedef map<long long,long long> mll;
typedef map<int,int> mii;
typedef map<char,long long> mcl;
typedef map<char,int> mci;
typedef map<string,long long> msl;
typedef map<string,int> msi;
typedef vector<long long> vl;
typedef vector<int> vi;
typedef vector<string> vs;
typedef vector<char> vc;
typedef vector<pair<int,int>> vpi;
typedef vector<pair<ll,ll>> vpl;
typedef vector<pair<string,string>> vps;
typedef vector<bool> vb;
bool is_prime(ll n) {
    if(n <= 1) {
        return false;
    }
    ll sqrt_n = sqrt(n);
    for(ll i = 2; i <= sqrt_n; i++) {
        if(n % i == 0) return false;
    }
    return true;
}
template <typename T>
set<T> intersect(const set<T> &s1, const set<T> &s2) {
    set<T> ans;
    for(const T &i : s1) {
        if(s2.count(i)) {
            ans.insert(i);
        }
    }
    return ans;
}

int main() {
    ios::sync_with_stdio(0);
    cin.tie(0);
    cout.tie(0);
    int t;
    cin >> t;
    while(t--) {
        int n;
        cin >> n;
        set<int> a;
        for (int i = 0; i < n; i++)
        {
            int x;
            cin >> x;
            a.insert(x);
        }
        cout << a.size() << "\n";
    }
    return 0;
}
```
- [x] Turn on GitHub Pages
- [ ] Outline my portfolio
- [ ] Introduce myself to the world
