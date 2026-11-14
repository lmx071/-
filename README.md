//顺序结构程序设计
//1001
#include<stdio.h>
int main()
{
    printf("zhe\n");
    printf("shi\n");
    printf("yi\n");
    printf("dao\n");
    printf("qian\n");
    printf("dao\n");
    printf("ti\n");
})

//1002
#include<stdio.h>
int main()
{
    printf("4396 = 28 x 157\n");
    printf("5346 = 18 x 297\n");
    printf("5346 = 27 x 198\n");
    printf("5796 = 12 x 483\n");
    printf("5796 = 42 x 138\n");
    printf("6952 = 4 x 1738\n");
    printf("7254 = 39 x 186\n");
    printf("7632 = 48 x 159\n");
    printf("7852 = 4 x 1963\n");
}
//1003

#include<stdio.h>
int main()
{
    printf("     **     \n");
    printf("     **     \n");
    printf("************\n");
    printf("************\n");
    printf("    *  *    \n");
    printf("    *  *    \n");
}
//1004

#include<stdio.h>
int main()
{
    printf("Helo word!");
}

//1005
#include<stdio.h>
int main()
{
    for(int i=1;i<=9;i++)
    {
        for(int j=1;j<=i;j++)
        {
            int k=j*i;
            if(j*i<10)
            {
                printf("%d*%d= %d",j,i,k);
                printf(" ");
            }
            else
            {
                printf("%d*%d=%d",j,i,k);
                printf(" ");
            }
        }
        printf("\n");
    }
}


//选择结构程序设计
A
#include<stdio.h>
int main(void)
{
    int a,b;
    scanf("%d %d",&a,&b);
    if (a<b)
       printf("<");
    if (a==b)
        printf("=");
    if (a>b)
        printf(">");
}  

B
#include <stdio.h>
int main(void)
{
	int n;
	scanf("%d",&n);
    if (n%2!=0)
        printf("%d",3*n+1);
    if (n%2==0)
        printf("%d",n/2);
    return 0;
}

C
#include <stdio.h>
int main(void)
{
	int a,b;
	scanf("%d %d",&a,&b);
    if (a==b){
        printf("Tacit！\n");      
    } else {
        printf("No Tacit!\n");   
    }
}

D
#include <stdio.h>
int main(void)
{
	int m,n;
	scanf("%d %d",&m,&n);
    if (m%n==0)
        printf("YES");
    if (m%n!=0)
        printf("NO");
    return 0;
}

E
#include <stdio.h>
int main(void)
{
	long x,y;
	scanf("%lld %lld",&x,&y);
    if (y%x==0){
        long z = x+y;
        printf("%lld\n",z);}
    else{
        long s = y-x;
        printf("%lld\n",s);}
    return 0;
}

//循环结构程序设计
1001
#include <stdio.h>
int main()
{
    int a,z;
    scanf("%d",&a);
    scanf("%d",&z);
    for(int i=1;i<=a;i++)
    {
    for(int b=1;b<=a-i;b++)
        printf(" ");
    for(int c=1;c<=2*i-1;c++)
        printf("*");
    printf("\n");
    }   
    for(int j=a-1;j>0;j--)
    {
        for(int d=1;d<=a-j;d++)
            printf(" ");
        for(int f=1;f<=2*j-1;f++)
            printf("*");
        printf("\n");
    }
     for(int i=1;i<=z;i++)
    {
    for(int b=1;b<=z-i;b++)
        printf(" ");
    for(int c=1;c<=2*i-1;c++)
        printf("*");
    printf("\n");
    }   
    for(int j=z-1;j>0;j--)
    {
        for(int d=1;d<=z-j;d++)
            printf(" ");
        for(int f=1;f<=2*j-1;f++)
            printf("*");
        printf("\n");
    }
}
    
1002
#include<stdio.h>
int main()
{
    int a,num=1;
    scanf("%d",&a);
    for(int i=1;i<=a;i++)
    {
        for(int j=1;j<=i;j++)
            printf("%4d",num++);
        printf("\n");
    }
}

1003
#include<stdio.h>
int main()
{
    char ch;
    scanf("%c",&ch);
    int a=ch-'A'+1;
    for(int i=1;i<=a;i++)
    {
        for(int j=1;j<=a-i;j++)
        
            printf(" ");
        for(int k=0;k<i;k++)
            printf("%c",'A'+k);
        for(int z=i-2;z>=0;z--)
            printf("%c",'A'+z);
        printf("\n");
    }
}

1004
#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    for(int i=1;i<=a;i++)
    {
        int j;
        scanf("%d",&j);
        for(int b=1;b<=(j+1)/2;b++)
        {
            for(int c=1;c<=(j+1)/2-b;c++)
                printf(" ");
            for(int d=1;d<=2*b-1;d++)
                printf("*");
            printf("\n");
        }
        for(int e=(j+1)/2-1;e>0;e--)
        {
            for(int f=1;f<=(j+1)/2-e;f++)
                printf(" ");
            for(int g=1;g<=2*e-1;g++)
                printf("*");
            printf("\n");
        }
    }
}

1005
#include<stdio.h>
int main()
{
    int a;
    while (scanf("%d", &a) != EOF)
    {
        for (int b = 1;b <= a + 1;b++)
        {
            for (int c = 1;c <= a + 1 - b;c++)
                printf("  ");
            for (int d = 1;d <= b;d++)
                printf("*");
            printf("\n");
        }
        for (int e = a;e > 0;e--)
        {
            for (int f = 1;f <= a + 1 - e;f++)
                printf("  ");
            for (int g = 1;g <= e;g++)
                printf("*");
            printf("\n");
        }
    }
}


//数组、字符串及数据批量存储
1001
#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>
int main()
{
   int T;
   scanf("%d", &T);
   while(T--)
    {
        int b,t;
        scanf("%d",&b);
        int c[b];
        for(int i=0;i<b;i++)
        {
            scanf("%d",&t);
            c[i]=t;
        }
        int max= c[0],min=c[0];
        long long num=0;
        for(int i=0;i<b;i++)
        {
            if(c[i]>max)
                max=c[i];
            if(c[i]<min)
                min=c[i];
            num+=c[i];
        }
        int j=max-min;
        double ave,sp=0.0;
        ave=(double)num/b;
        for(int i=0;i<b;i++)
        {
            double s=c[i]-ave;
            sp+=s*s;
        }
        double fancha=sp/b;
        printf("%d %.3lf",j,fancha);
        printf("\n");
    }
}

1002
#include <stdio.h>

int main() 
{
    int n, x;
    scanf("%d %d", &n, &x);
    int count = 0; 
    for (int i = 1; i <= n; i++) 
    {
        int temp = i;
        while (temp > 0) 
        {
            if (temp % 10 == x) 
            {
                count++;
            }
            temp /= 10; 
        }
    }
    printf("%d\n", count);
    return 0;
}

1003
#include <stdio.h>

int main() 
{
    int n, k, m;
    scanf("%d %d %d", &n, &k, &m);
    int in_queue[105]; 
    for (int i = 0; i < n; i++) 
    {
        in_queue[i] = 1;
    }
    int remaining = n;  
    int index = k;       
    int count = 0;       
    while (remaining > 1) 
    {
        if (in_queue[index] == 1) 
        {
            count++; 
            if (count == m) {
                in_queue[index] = 0; 
                count = 0;          
                remaining--;         
            }
        }
        index = (index + 1) % n; 
    }
    for (int i = 0; i < n; i++) 
    {
        if (in_queue[i] == 1) 
        {
            printf("%d\n", i);
            break;
        }
    }
    return 0;
}

1004
#include <stdio.h>
int main() 
{
    int L, M;
    scanf("%d %d", &L, &M);
    int tree[10005]; 
    for (int i = 0; i <= L; i++) 
    {
        tree[i] = 1;
    }
    for (int i = 0; i < M; i++) 
    {
        int l, r;
        scanf("%d %d", &l, &r);
        for (int j = l; j <= r; j++) 
        {
            tree[j] = 0;
        }
    }
    int count = 0;
    for (int i = 0; i <= L; i++) 
    {
        if (tree[i] == 1) 
        { 
            count++;
        }
    }
    printf("%d\n", count);
    return 0;
}

1005
#include <stdio.h>

int main() 
{
    int n;
    scanf("%d", &n);
    int prev, last;
    if (n == 1) 
    {
        scanf("%d", &last); 
    } else {        
        for (int i = 0; i < n; i++) 
        {
            if (i == n - 2) scanf("%d", &prev);
            else if (i == n - 1) scanf("%d", &last);
            else 
            {
                int temp;
                scanf("%d", &temp); 
            }
        }
    }
    if (n == 1) 
    {
        if (last == 0) printf("UP");
        else if (last == 15) printf("DOWN");
        else printf("-1");
    } 
    else 
    {
        if (last > prev) 
        { 
            if (last == 15) printf("DOWN"); 
            else printf("UP");
        } 
        else 
        { 
            if (last == 0) printf("UP"); 
            else printf("DOWN");
        }
    }
    return 0;
}


//函数与递归
A
#include <stdio.h>
int main() 
{
    int L, R, count = 0;
    scanf("%d %d", &L, &R);
    for (int i = L; i <= R; i++) 
    {
        int num = i;
        while (num > 0) {
            if (num % 10 == 2) count++;
            num /= 10;
        }
    }
    printf("%d", count);
    return 0;
}

B
#include <stdio.h>
int isLeap(int y) 
{
    return (y % 400 == 0) || (y % 4 == 0 && y % 100 != 0);
}

int countDigit(int n, int x) 
{
    int cnt = 0;
    if (n == 0) return (x == 0) ? 1 : 0;
    while (n > 0) 
    {
        if (n % 10 == x) cnt++;
        n /= 10;
    }
    return cnt;
}
int main() 
{
    int y, m, x;
    while (scanf("%d %d %d", &y, &m, &x) != EOF) 
    { 
        int days[] = {0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31};
        if (isLeap(y)) days[2] = 29;
        int total = 0;
        for (int d = 1; d <= days[m]; d++) 
        {
            total += countDigit(y, x);           
            int monthTens = m / 10;
            int monthOnes = m % 10;
            if (monthTens == x) total++;
            if (monthOnes == x) total++;         
            int dayTens = d / 10;
            int dayOnes = d % 10;
            if (dayTens == x) total++;
            if (dayOnes == x) total++;
        }
        printf("%d\n", total);
    }
    return 0;
}

C
#include <stdio.h>
#include <string.h>
#include <math.h>
int main() 
{
    char s[20];
    scanf("%s", s);
    int len = strlen(s);
    for (int i = len - 2, j = len; i >= 0; i--, j++) 
    {
        s[j] = s[i];
    }
    s[2 * len - 1] = '\0';
    long long num = 0;
    for (int i = 0; s[i]; i++) 
    {
        num = num * 10 + (s[i] - '0');
    }
    if (num < 2) 
    {
        printf("noprime");
        return 0;
    }
    int isPrime = 1;
    for (long long k = 2; k <= (long long)sqrt(num); k++) 
    {
        if (num % k == 0) {
            isPrime = 0;
            break;
        }
    }
    printf(isPrime ? "prime" : "noprime");
    return 0;
}

D
#include <stdio.h>
int digitSum(int n) 
{
    if (n < 10) 
    {
        return n;
    }
    return n % 10 + digitSum(n / 10);
}
int main() 
{
    int a, b;
    scanf("%d %d", &a, &b);
    int count = 0;
    for (int i = a; i <= b; i++) 
    {
        if (digitSum(i) % 5 == 0) 
        {
            count++;
        }
    }
    printf("%d", count);
    return 0;
}

E
#include <stdio.h>
#include <string.h>
void bigMul(char a[], char b[], int result[]) 
{
    int lenA = strlen(a);
    int lenB = strlen(b);
    int numA[55] = {0}, numB[55] = {0};
    for (int i = 0; i < lenA; i++) numA[i] = a[lenA - 1 - i] - '0';
    for (int i = 0; i < lenB; i++) numB[i] = b[lenB - 1 - i] - '0';
    memset(result, 0, sizeof(int) * (lenA + lenB));
    for (int i = 0; i < lenA; i++) {
        for (int j = 0; j < lenB; j++) 
        {
            result[i + j] += numA[i] * numB[j];
        }
    }
    for (int i = 0; i < lenA + lenB; i++) 
    {
        if (result[i] >= 10) 
        {
            result[i + 1] += result[i] / 10; 
            result[i] %= 10;                 
        }
    }
}

int main() 
{
    int T;
    scanf("%d", &T);
    while (T--) 
    {
        char a[55], b[55];
        scanf("%s %s", a, b);        
        int result[110] = {0};
        bigMul(a, b, result);
        int len = strlen(a) + strlen(b);
        int start = len - 1;
        while (start > 0 && result[start] == 0) 
        {
            start--;
        }       
        for (int i = start; i >= 0; i--) 
        {
            printf("%d", result[i]);
        }
        printf("\n");
    }
    return 0;
}


//栈、队列和stl
A
#include <stdio.h>
int a[8], used[9];
void dfs(int step) 
{
    int i;
    if (step == 8) 
    {
        for (i = 0; i < 8; ++i)
            printf("%d%c", a[i], i == 7 ? '\n' : ' ');  
        return;
    }
    for (i = 1; i <= 8; ++i) 
    {
        if (!used[i]) 
        {
            used[i] = 1;
            a[step] = i;
            dfs(step + 1);
            used[i] = 0;        
        }
    }
}

int main(void) 
{
    dfs(0);
    return 0;
}

B
#include <stdio.h>
#include <stdlib.h>
int cmp(const void *a, const void *b) 
{
    return (*(int*)b - *(int*)a);
}
int main() 
{
    int n, k;
    scanf("%d %d", &n, &k);
    int morning[100005], evening[100005];
    for (int i = 0; i < n; i++) scanf("%d", &morning[i]);
    for (int i = 0; i < n; i++) scanf("%d", &evening[i]);
    int diff[100005];
    long long total = 0; 
    for (int i = 0; i < n; i++) 
    {
        total += evening[i];
        diff[i] = morning[i] - evening[i]; 
    }
    qsort(diff, n, sizeof(int), cmp); 
    for (int i = 0; i < k; i++) 
    { 
        total += diff[i];
    }
    printf("%lld", total);
    return 0;
}

C
#include <stdio.h>
#include <stdlib.h>
int a[105];
int cmp(const void *pa, const void *pb) 
{
    int x = *(const int *)pa;
    int y = *(const int *)pb;
    if (x < y) return -1;
    if (x > y) return 1;
    return 0;
}
int main(void) 
{
    int n, i;
    scanf("%d", &n);
    for (i = 0; i < n; ++i) scanf("%d", &a[i]);
    qsort(a, n, sizeof(int), cmp);
    for (i = 2; i < n; ++i) 
    {
        if ((long long)a[i - 2] + a[i - 1] > a[i]) 
        {  
            printf("%d %d %d\n", a[i - 2], a[i - 1], a[i]);
            return 0;
        }
    }
    puts("No solution");
    return 0;
}

D
#include <stdio.h>
#include <string.h>
#include <stdlib.h>
char v[25][16];
char t1[32], t2[32];
int cmp(const void *pa, const void *pb) 
{
    const char *a = (const char *)pa;
    const char *b = (const char *)pb;
    strcpy(t1, a); strcat(t1, b);  
    strcpy(t2, b); strcat(t2, a);  
    return strcmp(t2, t1);         
}
int main(void) 
{
    int n, i;
    scanf("%d", &n);
    for (i = 0; i < n; ++i) scanf("%s", v[i]);
    qsort(v, n, sizeof(v[0]), cmp);
    for (i = 0; i < n; ++i) printf("%s", v[i]);
    putchar('\n');
    return 0;
}

E
#include <stdio.h>
#include <string.h>
int main() 
{
    char s[100005];
    scanf("%s", s);
    int len = strlen(s);
    if (len % 2 != 0) 
    {
        printf("Bad");
        return 0;
    }
    int cnt = 0;
    for (int i = 0; i < len; i++) 
    {
        if (s[i] == 'a') 
        {
            cnt++; 
        } else 
        {
            cnt--; 
            if (cnt < 0) 
            { 
                printf("Bad");
                return 0;
            }
        }
    }
    if (cnt == 0) 
    {
        printf("Good");
    } else {
        printf("Bad"); 
    }
    return 0;
}


//模拟、枚举与贪心
1001
#include <stdio.h>
#include <string.h>
static char s[200005];
int main(void) 
{
    int n, t, i, dot, end, p;
    if (scanf("%d %d", &n, &t) != 2) return 0;
    scanf("%s", s);
    int len = (int)strlen(s);
    dot = -1;
    for (i = 0; i < len; ++i)
        if (s[i] == '.') 
        { 
            dot = i; break; 
        }
    if (dot < 0) 
    { 
        puts(s); return 0; 
    }     
    end = len;
    p = -1;                                   
    for (i = dot + 1; i < len; ++i)
        if (s[i] >= '5') 
        { 
            p = i; break; 
        }
    while (t > 0 && p > dot) 
    {
        int j;
        end = p;                              
        j = end - 1;
        while (j >= 0) {                     
            if (s[j] == '.') 
            { 
                --j; continue; 
            }
            if (s[j] == '9') 
            { 
                s[j] = '0'; --j; 
            }
            else 
            { 
                ++s[j]; break; 
            }
        }
        if (j < 0) {                          
            memmove(s + 1, s, (size_t)end);
            s[0] = '1';
            ++end;
            ++dot;
        }
        --t;
        p = end - 1;                         
        if (!(p > dot && s[p] >= '5')) break;
    }
    s[end] = 0;
    while (end - 1 > dot && s[end - 1] == '0') --end;   
    if (end - 1 == dot) end = dot;                      
    s[end] = 0;
    puts(s);
    return 0;
}

1002
#include <stdio.h>
#include <string.h>
static int middle(int a, int b) 
{
    int r1 = (a - 1) / 3, c1 = (a - 1) % 3;
    int r2 = (b - 1) / 3, c2 = (b - 1) % 3;
    if (((r1 + r2) & 1) == 0 && ((c1 + c2) & 1) == 0) 
    {
        int r = (r1 + r2) / 2, c = (c1 + c2) / 2;
        int m = r * 3 + c + 1;
        if (m != a && m != b) return m;
    }
    return 0;
}
int main(void) 
{
    char s[64];
    while (scanf("%s", s) == 1) 
    {             
        int used[10] = {0};
        int ok = 1, i, len = (int)strlen(s);
        used[s[0] - '0'] = 1;
        for (i = 1; i < len; ++i) 
        {
            int d = s[i] - '0';
            int m;
            if (used[d]) 
            { 
                ok = 0; break; 
            }        
            m = middle(s[i - 1] - '0', d);
            if (m && !used[m]) 
            { 
                ok = 0; break; 
            } 
            used[d] = 1;
        }
        puts(ok ? "YES" : "NO");
    }
    return 0;
}

1003
#include <stdio.h>
static char s[20005];
int main(void) 
{
    int len = 0, c, i = 0;
    while ((c = getchar()) != EOF) s[len++] = (char)c;  
    while (i < len) 
    {
        if (s[i] == '"' && (i == 0 || s[i - 1] != '\\')) 
        {
            putchar(s[i]);
            ++i;
            while (i < len) 
            {
                putchar(s[i]);
                if (s[i] == '"' && s[i - 1] != '\\') 
                { 
                    ++i; break; 
                }
                ++i;
            }
        } else if (s[i] == '/' && i + 1 < len && s[i + 1] == '*') 
        {
            int j = i + 2;
            while (j + 1 < len && !(s[j] == '*' && s[j + 1] == '/')) ++j;
            if (j + 1 < len) 
            {
                i = j + 2;                
            } 
            else 
            {
                fwrite(s + i, 1, (size_t)(len - i), stdout); 
                i = len;
            }
        } 
        else 
        {
            putchar(s[i]);
            ++i;
        }
    }
    return 0;
}

1004
#include <stdio.h>
#include <string.h>
static char s[100005];
static const char *word[5] = {"zero", "two", "four", "six", "nine"};
static const char dig[5] = {'0', '2', '4', '6', '9'};
static const int wlen[5] = {4, 3, 4, 3, 4};
int main(void) 
{
    int T;
    scanf("%d", &T);
    while (T--) 
    {
        int i = 0, len, k;
        scanf("%s", s);
        len = (int)strlen(s);
        while (i < len) 
        {
            int done = 0;
            if (s[i] == '0' || s[i] == '2' || s[i] == '4'
                || s[i] == '6' || s[i] == '9') 
            {
                putchar(s[i]);                 
                ++i;
                continue;
            }
            for (k = 0; k < 5; ++k) 
            {
                if (i + wlen[k] <= len &&
                    strncmp(s + i, word[k], (size_t)wlen[k]) == 0) 
                {
                    putchar(dig[k]);          
                    i += wlen[k];
                    done = 1;
                    break;
                }
            }
            if (!done) ++i;
        }
        putchar('\n');
    }
    return 0;
}

1005
#include <stdio.h>
int main(void) 
{
    int cnt[10], i, k, odds = 0;
    char left[105], ans[210];
    int hn = 0, p = 0, first = -1, center = -1;
    for (i = 0; i < 10; ++i) 
    {
        scanf("%d", &cnt[i]);
        if (cnt[i] & 1) 
        { 
            ++odds; center = i; 
        }
    }
    if (odds > 1) 
    { 
        puts("-1"); return 0; 
    }  
    for (i = 0; i < 10; ++i)                  
        for (k = 0; k < cnt[i] / 2; ++k)
            left[hn++] = (char)('0' + i);
    if (hn == 0) 
    {                           
        for (i = 0; i < 10; ++i)
            if (cnt[i]) { printf("%d\n", i); return 0; }  
        puts("-1");
        return 0;
    }
    for (i = 0; i < hn; ++i)                  
        if (left[i] != '0') 
        { 
            first = i; break; 
        }
    if (first < 0) 
    { 
        puts("-1"); return 0; 
    }  
    ans[p++] = left[first];                  
    for (k = 0; k < cnt[0] / 2; ++k) ans[p++] = '0';   
    for (i = 0; i < hn; ++i) 
    {               
        if (i == first || left[i] == '0') continue;
        ans[p++] = left[i];
    }
    if (odds == 1) ans[p++] = (char)('0' + center);   
    for (i = p - 1 - (odds == 1); i >= 0; --i)       
        ans[p++] = ans[i];
    ans[p] = 0;
    puts(ans);
    return 0;
}
