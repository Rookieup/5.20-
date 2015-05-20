#include <stdio.h>
int main()
{
    //定义6个变量存放学生的成绩
    int a =0,b =0, c=0 , d = 0;
    
    //提示学生输入四科成绩
    printf("请输入你的四科成绩,用逗号隔开:\n");
    //接收学生的四科成绩
    scanf("%d,%d,%d,%d",&a,&b,&c,&d);
    int max=a,min=a;
    //判断学生的成绩高低
    if (b > max) {
        max = b;
    }
    if (c > max){
        max = c;
    }
    if (d > max){
        max = d;
    }else {
        max = a ;
    }
    //判断最小值
    if (b < min) {
        min = b;
    }
    if (c < min){
        min = c;
    }
    if (d < min){
        min = d;
    }else{
        min = a;
    }
    
    printf("max=%d,min=%d",max,min);
    return 0;
}
