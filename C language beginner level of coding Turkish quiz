#include <stdio.h>
#include <string.h>
void hosgeldinizFonksiyonu(){
	printf("Fatih Ates Bilgi yarismasina hosgeldiniz. Lutfen asagidaki kurallari okuyunuz\n"
	"***Yarismamiz puan sistemlidir\n***Lutfen kullanici adinizi dogru giriniz, kayitli degilseniz uye olunuz.");
}
int secimFonksiyonu(){
	int secim;
	printf("\nLutfen asagidaki seceneklerden birini seciniz\n[1]-Giris Yap\n[2]-Kayit ol\n");
	scanf("%d",&secim);
	return secim;
}
int girisYapFonksiyonu(char isim[40],char sifre[40]){
	char isimVeri[40];
	char sifreVeri[40];
	bool kontrol=false;
	while (kontrol==false){
		
	printf("Lutfen adinizi giriniz:");
	scanf("%s",&isimVeri);
	printf("Lutfen sifrenizi giriniz:");
	scanf("%s",&sifreVeri);
	if(strcmp(isim,isimVeri)==0 && strcmp(sifre,sifreVeri)==0){
		printf("Sisteme hosgeldiniz\n");
		kontrol=true;
	}
	else{
		printf("Hatali giris\n");
	}
}
}
int kayitOlFonksiyonu(){
	char isim[40];
	char sifre[40];
	printf("Lutfen bir isim belirleyiniz:");
	scanf("%s",&isim);
	printf("Lutfen bir sifre belirleyiniz:");
	scanf("%s",&sifre);
	printf("Basarili bir sekilde kaydiniz gerceklesti.\n****Giris ekranina yonlendiriliyorsunuz.****\n");
	girisYapFonksiyonu(isim,sifre);
}
int bilgiYarismasi(){
	char cevap[2];
	int puan=0;
	int can=3;
	printf("Yarisma basladi\n");
	printf("Puaniniz:%d",puan);
	while(can!=0){
	if(puan==0){
	
	printf("\n[Soru-1]Asagidakilerden hangisi Kazakistan'in baskentidir?\nA-)Biskek\nB-)Otuken\nC-)Nur-Sultan\nD-)Taskent\n");
	scanf("%s",&cevap);
	if(strcmp(cevap,"C")==0){
		printf("Dogru cevap\n");
		puan+=10;
		printf("Puaniniz:%d",puan);
	}
	else
	{
		printf("Hatali cevap verdiniz.\n");
		printf("\npuan:%d",puan);
		can=can-1;
		printf("\nCaniniz:%d\n",can);
	}
	
}
if (puan==10){
	printf("\n[Soru-2]Asagidakilerden hangisi ABD'nin Kalifornya eyaletinde bulunan sehirlerinden birisi degildir?\nA-)Los Angeles\nB-)Los Santos\nC-)San Diego\nD-)San Francisco\n");
	scanf("%s",&cevap);
	if(strcmp(cevap,"B")==0){
			printf("Dogru cevap\n");
		puan+=10;
		printf("Puaniniz:%d",puan);
	}
	else
	{
			printf("Hatali cevap verdiniz.");
		printf("\npuan:%d",puan);
		can=can-1;
		printf("\nCaniniz:%d\n",can);
	}
}
if (puan==20){
	printf("\n[Soru-3]Asagidakilerden hangisi 1. Dunya Savasi'nda Osmanli Devleti'nin muttefiklerinden biri degildir?\nA-)Sirbistan\nB-)Bulgaristan\nC-)Avusturya-Macaristan\nD-)Almanya\n");
	scanf("%s",&cevap);
	if(strcmp(cevap,"A")==0){
			printf("Dogru cevap\n");
		puan+=10;
		printf("Puaniniz:%d",puan);
		can=0;
	}
	else
	{
			printf("Hatali cevap verdiniz.");
		printf("\npuan:%d",puan);
		can=can-1;
		printf("\nCaniniz:%d\n",can);
	}
}
}
return puan;
}

int yarismaSon(int puan){
	printf("\nYarismamiz sona ermistir.\nGuncel puaniniz:%d\nYine bekleriz...",puan);
}

int main(){
	char isim[40]="FatihAtes";
	char sifre[40]="200022";
	hosgeldinizFonksiyonu();
	int secim=secimFonksiyonu();
	if(secim==1){
		girisYapFonksiyonu(isim,sifre);
	}
	else if(secim==2){
		kayitOlFonksiyonu();
		}
	int skor=bilgiYarismasi();
		yarismaSon(skor);
	
	return 0;
}
