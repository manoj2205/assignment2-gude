# assignment2-gude
Assignment-2 is started
# MANOJ KUMAR GUDE
###### vijayawada food court
In the vijayawada food court we can have different types of **biryanis**, noodles, deserts and **shawaramas**
---
# FOOD MENU
VIJAYAWADA INTERNATIONAL AIRPORT
1. Reach outside to the terminal and look for a cab
2. Tell the cab driver to go Vijayawada benz circle
3. Tell him to move forward for 500m, then you can see Nalanda college on the right side
4. Drop there and move toward Nalanda college
5. When you reached Nalanda college there you can see Eat Street board, that means you reached.

* Cola
* Rayalaseema NatuKodi Biryani
* RagiSangati NatuKodi Pulusu
* Punugulu
* Bajji
    * Masala Bajji
    * Vankaya Bajji
    * Chilli Bajji
    * Egg Bajji
[AboutMe](https://github.com/manoj2205/assignment2-gude/blob/main/AboutMe.md)
---
| Sport | Location | Personel_Equipment_Charge |
| ----- | -------- | ------------------------- |
| Volley_Ball | University_Rec | $10 |
| Batminton | University_Rec | $20 |
| Cricket | University_PlayGround | $50 |
| Basket_Ball | University_Rec| $25 |
---
# Pithy Quotes
> Never Giveup! - *MANOJ_KUMAR_GUDE*

> Sometimes life hits you in the head with a brick. Don't lose faith. - *Steve_Jobs*
---
# Code_Fencing
> The convex hull may be defined either as the intersection of all convex sets containing a given subset of a Euclidean space, or equivalently as the set of all convex combinations of points in the subset. 
[Geometry Convex hull](https://en.wikipedia.org/wiki/Convex_hull)
``` 
const int maxn = 2e5;

point line[4 * maxn];

void add_line(point nw, int v = 1, int l = 0, int r = maxn) {
    int m = (l + r) / 2;
    bool lef = f(nw, l) < f(line[v], l);
    bool mid = f(nw, m) < f(line[v], m);
    if(mid) {
        swap(line[v], nw);
    }
    if(r - l == 1) {
        return;
    } else if(lef != mid) {
        add_line(nw, 2 * v, l, m);
    } else {
        add_line(nw, 2 * v + 1, m, r);
    }
}

```
<https://cp-algorithms.com/geometry/convex_hull_trick.html>