#include<stdio.h>
int x[8];
int Place(int k,int i)
{   int j;
    for(j=1;j<=k-1;j++)
    {
        if((x[j]==i)||((Abs(x[j]-i))==Abs(j-k)))
        {
            return 0;
        }
    }
 return 1;
}
int Abs(int g)
{
    if(g<=0)
    {
        return (-g);
    }
    else
    return (g);
}
void NQueen(int p,int q)
{ int i,e=0;
    for(i=1;i<=q;i++)
    {
        if(Place(p,i))
        {
            x[p]=i;
            if(p==q)
            {   printf("order:");
                e++;
                for(i=1;i<=q;i++)
                {
                    printf("%d",x[i]);
                    printf(" ");
                }
            }
            else
            {
                NQueen(p+1,q);
            }
        }
    }
}
int main()
{
    NQueen(1,4);
}
