# baitapmang
#include<stdio.h>
#include<conio.h>
#include<string.h>
int giaithua(int n){
	int i, gt=1;
    for(i = 1; i <= n; i++)
    {
        gt*=i;
    }
   	return gt; 
}
int main(){
	int n,i,j,s=0;
	//bài 1
	printf("Nhap so phan tu cua mang: ");
	scanf("%d",&n);
	int a[n];
	for ( i = 0; i < n; ++i){
		printf("a[%d] = ",i);
		scanf("%d",& a[i]);		
	}
	//bài 2
	printf("Mang ban vua nhap :\n");
	for (int i = 0; i < n ; ++i)
		printf(" a[%d]= %d\n",i,a[i]);
	
	//bàI 3
	for (j=0 ; j<n ;j++){
		s=s+giaithua(a[j]);
	}
	printf("tong giai thua cac phan tu cua mang: s=%d",s);
	//bài 4
	char chuoi[100];
	printf("\nNhap vao chuoi bat ky :");
	scanf("%s",chuoi);
	int k=0,dem=0;
	while(k<10){
		if(chuoi[k]!='\0') dem++;
		else break;
		k++;
	
	}
	printf("Chuoi ban da nhap co %d ky tu",dem);
	return  0;
		
}


