---
title: "CodeForce Problem Solving in C Part 1"
layout: post
date: 2022-01-5 22:10
tag: problem-solving
image: 
headerImage: true
projects: true
hidden: false 
description: ""
category: project
author: johndoe
externalLink: false
---

[GitHub Repository](https://github.com/tarekfouad97/CodeForce-Problem-Solving)

---

[Anton and Danik](https://codeforces.com/contest/734/problem/A)   
{% highlight %}
#include <stdio.h>

int main()
{
    int n;
    int a_counter = 0;
    int d_counter = 0;
    char result;
    scanf("%d", &n);

    for (int i = 0; i != n; i++)
    {
        scanf("%c", &result);
        if (result == 'A')
        {
            a_counter++;
        }
        else if (result == 'D')
        {
            d_counter++;
        }
    }

    if (a_counter < d_counter)
    {
        printf("Danik");
    }
    else if (a_counter > d_counter)
    {
        printf("Anton");
    }
    else if (a_counter == d_counter)
    {
        printf("Friendship");
    }
    return 0;
    
}
{% endhighlight %}
---
[Bear and Big Brother](codeforces.com\contest\791\problem\A)    
{% highlight html %}
#include <stdio.h>

int main()
{
    int bear;
    int brother;
    int years=0; //assign it to zero

    scanf("%d", &bear);
    scanf("%d", &brother);
    while (1)
    {
        bear *= 3;
        brother *= 2;
        years++;
        if (bear > brother)
        {
            break;
        }
    }
    printf("%d",years);
}

{% endhighlight %}
---
[Team](https://codeforces.com/contest/231/problem/A)      
{% highlight html %}
#include <stdio.h>

int main()
{
    int Petya, Vasya, Tonya;
    int problem;
    int sum;
    int count=0;
    scanf("%d", &problem);
    int i;
    for (i = 0; i < problem; i++)
    {
        sum = 0;
        scanf("%d %d %d", &Petya, &Vasya, &Tonya);
        sum = Petya + Vasya + Tonya;

        if (sum == 3 || sum == 2)
        {
            count++;
        }
    }
    printf("%d", count);
}
{% endhighlight %}

---
[Beautiful Matrix](https://codeforces.com/contest/263/problem/A)  
{% highlight html %}
#include <stdio.h>
#include <stdlib.h>

int main()
{

    int matrix[5][5];
    int i, j;
    int i_location=0;
    int j_location=0;
    int result=0;

    for (i = 0; i < 5; i++)
    {
        for (j = 0; j < 5; j++)
        {

            scanf("%d ", &matrix[i][j]);
        }
    }
    if (matrix[2][2] == 1)
    {
        printf("0");
        return 0;
    }
    else
    {
        for (i = 0; i < 5; i++)
        {
            for (j = 0; j < 5; j++)
            {
                if(matrix[i][j] == 1){
                    
                    i_location=3-(i+1);
                    j_location=3-(j+1);
                    result= abs(i_location)+abs(j_location);
                    printf("%d",result);
                    break;
                }
            }
        }
    }
    return 0;
}
{% endhighlight %}
---
[Gravity Flip](https://codeforces.com/contest/405/problem/A)     
{% highlight html %}

{% endhighlight %}
---
[Petya and Strings](https://codeforces.com/contest/112/problem/A)  
{% highlight html %}
#include <stdio.h>
#include <string.h>
int main()
{

    char x[200];
    char y[200];

    scanf("%s", x);
    scanf("%s", y);

    for (int i = 0; i < strlen(x); i++)
    {
        if (x[i] < 92)
        {
            x[i] += 32;
        }
        if (y[i] < 92)
        {
            y[i] += 32;
        }
    }

    int count = 0;
    while (x[count] != '\0' && y[count] != '\0')
    {

        if (x[count] > y[count])
        {
            printf("1");
            return 0;
        }
        else if (x[count] < y[count])
        {
            printf("-1");
            return 0;
        }
    
        count++;
    }
    printf("0");
    return 0;
}
{% endhighlight %}
---
[Boy or Girl](https://codeforces.com/contest/236/problem/A)  
{% highlight html %}
#include <stdio.h>
#include <string.h>

int main()
{

    char str[100];
    int count = 0;
    int result = 0;
    scanf("%s", str);

    int size = 26;
    int arr[size];
    for (int i = 0; i <= size; i++)
    {
        arr[i] = 0;
    }
    int temp = 0;
    for (int i = 0; str[i] != '\0'; i++)
    {
        temp = str[count] - 'a';
        arr[temp]++;

        count++;
    }
    for (int i = 0; i <= size; i++)
    {
        if (arr[i] >= 1)
        {
            result++;
        }
    }
    
    if (result % 2 == 0)
    {
        printf("CHAT WITH HER!");
    }
    else
    {

        printf("IGNORE HIM!");
    }
    return 0;
}
{% endhighlight %}
---
[Word]()    
{% highlight html %}

{% endhighlight %}
---
[Magnets]() 
{% highlight html %}

{% endhighlight %}
---
[Sereja and Dima]()    
{% highlight html %}

{% endhighlight %}
---
