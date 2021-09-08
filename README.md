# Assignment2_Harshita
# Harshita
###### Hyderabad 

It is my hometown, it is famous for Biryani and **Golkonda** it is also one of the **metropolitan** city in India

--------
# Way to Hyderabad

1. Check your savings or bank balance for planning a trip
2. Get visa from India to visit Hyderabad
3. Book a flight to India, RGV In Airport.
    1. Book a hotel stay.
    2. Book a cab from airport to hotel.
4. visit the near by places and have nice biryani. 


## Unordered list

* Car to travel
* Food items
    * maggi
    * popcorn
    * pepsi
* chess board, valley ball to play
* Nice camera for pictures

[Aboutme](https://github.com/HarshitaGITHB/Assignment2_Harshita/blob/main/AboutMe.md)

--------

# FOOD Recommendations

Below iteams are the items which i have tried in Maryville and Kansas. I liked few of them and few i didnot. Few of the items are cost worthy and few not. 

|  food               |   location     |   price   |
|---------------------|--------------- |-----------|
| Instant noodles     | Dollar general |   $1.99   |
| Egg roles           |  Thai corner   |   $4.00   |
| chicken fry biryani |   godavari     |  $32.00   |
|  French fries       |   Mac D        |   $4.00   |

-------------
# Qutoes

> "Be yourself; everyone else is already taken" - *Oscar Wilde*

> “Two things are infinite: the universe and human stupidity; and I'm not sure about the universe." - *Albert Einstein*

------------

# Code Fencing

> In computer science, a suffix array is a sorted array of all suffixes of a string. It is a data structure used in, among others, full text indices, data compression algorithms, and the field of bibliometrics. ... The suffix array for a subset of all suffixes of a string is called sparse suffix array.

FormoreInfo >https://en.wikipedia.org/wiki/Suffix_array>

```
 vector<int> pn(n), cn(n);
    for (int h = 0; (1 << h) < n; ++h) {
        for (int i = 0; i < n; i++) {
            pn[i] = p[i] - (1 << h);
            if (pn[i] < 0)
                pn[i] += n;
        }
        fill(cnt.begin(), cnt.begin() + classes, 0);
        for (int i = 0; i < n; i++)
            cnt[c[pn[i]]]++;
        for (int i = 1; i < classes; i++)
            cnt[i] += cnt[i-1];
        for (int i = n-1; i >= 0; i--)
            p[--cnt[c[pn[i]]]] = pn[i];
        cn[p[0]] = 0;
        classes = 1;
        for (int i = 1; i < n; i++) {
            pair<int, int> cur = {c[p[i]], c[(p[i] + (1 << h)) % n]};
            pair<int, int> prev = {c[p[i-1]], c[(p[i-1] + (1 << h)) % n]};
            if (cur != prev)
                ++classes;
            cn[p[i]] = classes - 1;
        }
        c.swap(cn);
    }
    return p;
}
```
FormoreInfo <https://cp-algorithms.com/string/suffix-array.html>

